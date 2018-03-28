
# Object-Oriented Analysis and Design
## Overview

With the functional requirements of the THS established and use cases developed to model the user interaction with the system, it was necessary to begin to move from the problem domain to the solution domain and move more towards the language of the developer, structured by classes and packages rather than use cases. [1]  
 
In doing so, the domain model and use cases were analysed to identify the key objects to be modelled in the system. With the objects identified, the data attributes of the objects and method call sequences required to realise the use cases were established through an iterative process of role play and pseudo-code development. This resulted in an analysis class diagram - showing the key objects and their relationships, a design class diagram – a more comprehensive and defined representation of the system’s classes, sequence and activity diagrams, state machine diagrams and a deployment diagram, which will be discussed in the following sections. 

## Activity Diagrams

Activity diagrams help to model system processes through a series of activities. They have convenient notation, similar to flow charts and can be thought of as Object Oriented flowcharts. [9] Unlike class diagrams or sequence diagrams, actions are written in plain English as these diagrams serve as predecessors to more complex, class-oriented models. 

The THS team used activity diagrams to model complete processes including both software and real-world activities, and in doing so indicated the relationship between such activities and how they are carried out to fulfill system requirements. Included in these representations are start and stop states, indicating the beginning and end of an activity and forks and joins, to illustrate when activity states occur concurrently. [9] Alternative flows are modeled by decisions, represented by a diamond, and indicate different flow directions that can be taked based on a certain condition. The final iterations of activity diagrams for the THS are shown below as well as a key to activity diagram syntax. 

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.6\textwidth]{TempImg/ADKey.png}
      \caption{Key for activity diagram symbols}
 \end{figure}



 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.65\textwidth]{TempImg/makeOrderAD.png}
      \caption{Activity diagram for UC7:Creates Order}
 \end{figure}

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.6\textwidth]{TempImg/newUserAD.png}
      \caption{Activity diagram for UC1: Creates Account}
 \end{figure}

  \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.9\textwidth]{TempImg/checkoutAD.png}
      \caption{Activity diagram for UC8: Checks Out}
 \end{figure}


  \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.45\textwidth]{TempImg/manageToolsAD.png}
      \caption{Activity diagram for UC6: Manages Tool Listings}
 \end{figure}


## UML Class Diagrams 

### Analysis Class Diagram

A use case driven approach was used to identify the key nouns and verbs and iteratively develop these into the system’s objects and method calls. The analysis class diagram in Figure 4.7 shows a middle stage iteration. The classes are labelled as either boundary, controller or entity classes in line with the Jacobson categorisation style [10]. In this style, the boundary classes encapsulate output data and generates output in the required form, the controller classes deal with controlling behaviour and completing tasks and the entities classes store the data and define operations on the data. The advantage of this is that it enforces clear partitioning of responsibilities in the class structure early on in the object-oriented design process.  
 
The class names were kept close to the functionality of the class which will allow for clarity in the development phase. The relationships (associations, generalisations, dependencies, aggregations and compositions) were mapped between the classes only where a relationship was necessary to achieve a use case.

\begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/OOClass.png}
      \caption{A model of Boundary-Control-Entity architecture [11]}
 \end{figure}

\begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.6\textwidth]{TempImg/DClassKey.png}
      \caption{Class diagram key}
 \end{figure}

  \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.99\textwidth]{TempImg/AClass.png}
      \caption{Analysis Class Diagram}
 \end{figure}

### Design Class Diagram

The analysis diagram was used as a basis to build the design class diagram, which specifies in more detail how the system will be implemented, getting closer to the solution domain. There was a strong focus on adhering to object-oriented principles. Some of the considerations that went into the design class diagram are discussed here:

#### Adding Implementation Details

Variable types, method parameters and return types were added, along with variable and method visibility. Adhering the object-oriented principle of \textbf{encapsulation} most class member variables were given private visibility with public methods that allow access to them. (NB for the sake of coherence of the diagram, not all getters and setter were modelled for every class). 

\textbf{Static methods} were also used where there was no need for the method to use instance variables and the method therefore belongs to the class rather than an instance of the class. For example - the methods in the database connector are static, as is the ‘connectionStatus’ variable. This makes the class a \textbf{singleton class} [12] whereby only one instance of the class need exist in the Java Virtual Machine and providing a global point of access to other classes that need it. 

\textbf{Inheritance} was used only where needed – to generalise a customer and employee to a user – thereby eliminating duplication of user details in each class. It was also used in the ‘PaymentMethod’ (parent) and ‘Deposit’ (child) relationship.

\textbf{Interfaces} were used to help separate the specification of an entity from implementation of a task. For example - the employee controller manages a tool listing via a ‘manageToolListing’ interface. This has the advantage that in the future, should the GUI for the tool listing change, it is easier to change the implementation of the ‘manage tool listing’ methods.

#### Completeness & Primitiveness

\textbf{Completeness: } this is the specification that the design classes should cover all the data and functionality needed. We ensured this by iteratively mapping out use case flows and ensuring that classes are related and can therefore access instances of each other when required. Classes were also added from the analysis class where needed.

\textbf{Primitiveness:} this is the specification that there should never be more than one way of doing things. For example – in our system there is just a single ‘respondToQuery()’ method that encompasses different types of query rather than several separate methods. 

#### High Cohesion & Low Coupling

\textbf{High cohesion: } this specifies that each class should model a single abstract concept [9]. We ensured this by separating out the implementation for managing queries/blog/tool listing/shopping basket/user accounts – so that the employee and customer controllers do not take on several different responsibilities. This is also the case for the database connector which is a simple class, just concerned with connecting to the database, the create/read/update methods are present in the respective entities. 

\textbf{Low coupling: }This specifies that classes should associate with just enough other classes to realise its goal – e.g. which was achieved by using focused aggregation rather than inheritance in most places. 

\begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.85\textwidth]{TempImg/Dclass.png}
      \caption{Design Class Diagram}
 \end{figure}

Below, there is a class table describing the functionality of the classes in this model.

\begin{table}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.9\textwidth]{TempImg/CT1.png}
\end{table}

\begin{table}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.9\textwidth]{TempImg/CT2.png}
      \caption{Class table describing the funtionality of classes in the THS system.}
\end{table}


Additionally, earlier iterations of the design class diagram can be seen in Appendix 8.2. 

## Sequence Diagrams

Sequence diagrams serve as the bridge between use cases and class diagrams. They are a type of interaction diagram which describes the order in which interactions in a system occur. The events in sequence diagram are shown chronologically, with the earliest event at the top of the diagram and the last event at the bottom. Events occur between participants, which in the case of the THS, are actors,  databases, and classes derived from the class diagram. Each event has a message which describes the interaction between participants. Methods from the design class diagram are used as messages and allow the classes to interact. Interactions between the actors and boundaries have messages given in pseudo code to describe the real-world interaction between the user and the interface. [9]

For the purposes of this project, messages were given without arguments. Given that team determined that the diagrams were useful and adequately descriptive using this high level approach, the arguments were intentionally left out to reduce clutter. Six sequence diagrams are given below to illustrate some of the most relevant use cases in addition to a key describing the features that appear. For early iterations of key sequence diagrams, please see Appendix 8.3.  

\begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.6\textwidth]{TempImg/SDKey.png}
      \caption{Sequence diagram symbol key}
\end{figure}

\begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/add_new_tool_SD.png}
      \caption{Sequence diagram for adding a new tool listing to the THS system. This is a version of UC6: Manages Tool Listing}
\end{figure}

\begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/new_user_reg_SD.png}
      \caption{Sequence diagram for registering a new customer to the THS system. This is a version of UC1: Creates Account}
\end{figure}

\begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.8\textwidth]{TempImg/create_order_SD.png}
      \caption{Sequence diagram for creating an order in the THS system. This is a version of UC7: Creates Order}
\end{figure}

\begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=1.1\textwidth]{TempImg/check_out_SD.png}
      \caption{Sequence diagram for checking out. This is a version of UC8: Checks Out}
\end{figure}

\begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.8\textwidth]{TempImg/make_blog_post_SD.png}
      \caption{Sequence diagram for an admin creating a blog post. This is a version of UC23: Posts Advice Blog & Video Tutorials}
\end{figure}

\begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.8\textwidth]{TempImg/make_query_SD.png}
      \caption{Sequence diagram for a customer entering a query into the THS system. This is a version of UC19: Raises Query}
\end{figure}




## State Machine Diagram

In this section three state machine diagrams are displayed and explained. 

#### Tool Rental Lifecycle

This diagram represents the lifecycle of a tool hire from the perspective of the tool itself. The tool can switch between four states which are: \textit{Available, Booked, Serviced and Maintained}. The lifecycle begins at the available state. After the tool is booked by a client the tool changes its state to booked. Subsequently, once the tool is returned it is checked on functionality and observable flaws. Consequently, the tool is either serviced, if it needs repair or it is put back in the state of maintained. After this last step, the tool is ready for rental again and the state of the tool is changed to available. This closed the cycle and the loop continues. 

\begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.8\textwidth]{TempImg/ToolSM.png}
      \caption{State machine diagram for a tool rental}
\end{figure}

#### Order

This diagram visualises the five different states from the shipping perspective. The five states are: \textit{Pending, Packed, Dispatched, Delivered, Returned and Closed.} 

Once the client completed his order, the order changes its state to pending, after the shipping is initialized the state of the order is changed to packed. Consequently, the ordered tool will be dispatched. If the order could not be delivered, it will be returned and dispatched again. Once the shipping is completed it will change its state to delivered. As soon as the order is cleared the order will change to the final state, which is the closed status. 

\begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.8\textwidth]{TempImg/OrderSM.png}
      \caption{State machine diagram for an order}
\end{figure}

#### Shopping Basket

The following state machine diagrams displays the four stages of the shopping basket. The four states are: \textit{Empty, Collecting, Checked Out and Ordered.}

The initial state of the shopping basket is empty, once tools are added it changes to the collecting state, if the added tool is deleted again we find ourselves again in the empty state.In the collecting state, arbitrarily many products can be added or deleted. As soon as 1 product is in the basket, the collecting state is initialized.  Once the client confirms that the order the status is updated to checked out. If the summary is accepted the shopping basket will convert to the final state ordered. However, if the order is abandoned, the whole basket will be cleared and it goes back to the initial state, empty.

\begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.8\textwidth]{TempImg/BasketSM.png}
      \caption{State machine diagram for a shopping basket}
\end{figure}


## Component Diagram

Figure 4.19 shows the component diagram, which indicates a static representation of the projected system with regards to the logical elements. This diagram represents part of the architectural features of the system. It is more abstract, and it has less details than the previous class and object-oriented diagrams, therefore, it helps to familiarize the viewer with the system architecture. The DIY Tool Hire Service component diagram has four fundamental but interconnected groups. 

Groups of the components in the DIY Hire Service system:


\begin{itemize}
  \item \textbf{Components related to the User interaction.} It allows the users to interact with the system. We have a browser engine, that allow users to find the products; shopping basket, which manage client’s tools basket and the User Session, such as the log-in process.
  \item \textbf{Components related to the Warehouse management.} It manages which tools are available and in which quantity.
  \item \textbf{Components related to the Payment System.} It interacts with the APIs of several third-party payment services, such as Visa, MasterCard, PayPal. It allows to complete the transaction
  \item \textbf{Components related to the Administration control.} It controls the Orders flow and consequentially it depends on the other components. 
\end{itemize}
	

Each of the above stated groups includes of components of various types such as: executables, libraries, files, ports, connectors and interfaces. The figure below shows the components diagram which complies with UML 2.0 notation standard.

\begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.9\textwidth]{TempImg/compD.png}
      \caption{System components diagram}
\end{figure}


## Three Tier Architecture

A three tier model partitions a system’s component’s into three layers of services. These are more a representation of the logical tiers in a system as opposed to a direct physical representation. 

The outermost tier that is responsible for user interaction with the system is called the Presentation Tier. [13] For the Tool Hire Service, this means the website’s interface with which the user interacts. Through the use of Dynamic HTML a THS customer or employee can interact with the services in the second tier in a simple and intuitive manner. 
The second tier is known as the Logic or Business Services layer. The processes contained in the second tier carry out the actual logic and functionality of the application and have access to the third tier. Since many clients can access this tier from different devices simultaneously, it is important that this tier manages its transactions in order to keep the data structures in the third tier consistent and reliable. [14] An example of how this may be used in the THS system would be if multiple customers were trying to book a tool at the same time. The logic tier must be able to “decide” which customer will get to rent the tool, update the database, and send a message to each customer indicated the result. Managing such conflicts in the second tier greatly reduces the burden on the third tier services. [13]

Finally, the third and innermost tier comprises of a system’s data. The database management system (DBMS) and the data it manages can only be accessed via the second tier. [13] This is where all data for the system is stored. In the case of the THS, some example of data stored here would be Order data, Customer data and Tool data. Access to this layer can be seen in the design class diagram as the DBConnector class.

\begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.9\textwidth]{TempImg/3TA.png}
      \caption{Three tiers for the THS system}
\end{figure}

Even though this architecture is more complex than a single tier, the benefits of using a three tier architecture outweigh the drawbacks. The three most important reasons a three tier architecture is suitable for the THS are:

\begin{itemize}
  \item If the THS were to expand, the system is easily scalable since the data layer is independent from the other two.

  \item It is easier to maintain and modify the underlying code of the system if it is divided into separate layers, for example the UI can change without modifying the logic layer.

  \item Increased security with security defined for each layer. Since users can only access the second tier and not the third, if proper security measures are taken, a three tier architecture is more secure than a two tier architecture. However, having an additional tier means that during system development, security measure must be carefully discussed between developers working of different tiers in order to ensure that increased surface area doesn’t lead to increased risk. 

\end{itemize}

## Deployment Diagram

The Deployment Diagram shown in Figure 4.21 shows the deployment of various software artefacts generated by the Tool Hire Service (THS) to deployment targets.  Deployment targets are called nodes and can represent a device such as a computer or a software execution environment. The deployment diagram shows the full hardware architecture of the THS. Included is the customer’s desktop, a webserver, an application server and finally a database. The customer’s pc connects to the web server where the website is hosted via HTTP (Hypertext Transfer Protocol). The web server then connects to the application server via RMI (Remote Method Invocation) which handles the business logic for components such as orders, shipping and blog posts. Lastly the application server connects to the database via JDBC (Java database connectivity).

\begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.6\textwidth]{TempImg/depD.png}
      \caption{Deployment diagram}
\end{figure}



\newpage