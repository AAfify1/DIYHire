# Project Overview


## Team Members

\begin{table}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.6\textwidth]{TempImg/teamtable.png}
      \caption{Team members and email addresses}
\label{conreq}
 \end{table}

## Introduction

This report will elaborate on the process used by Group A to design the DIY Tool Hire Service.  The assignment was completed following the use-case driven Unified Software Development Process (USDP)[1].  

The iterative nature of the USDP resulted in multiple evolutions at every step in the process.  While each aspect of development – from the requirements gathering and use cases to the object-oriented diagrams – underwent several iterations, only the final iterations have been included within the report.  All of the core diagrams found in this report were completed in Unified Modeling Language (UML) format, the industry standard.

This chapter of the report will contain the problem statement, a description of the scope of the project, a glossary of terms used throughout the report, and a Gantt chart to display the project timeline followed by the team.  Following these sections is a summary of the project management style. The subsequent chapters will cover the topics of requirements gathering, use case development, object-oriented analysis, and application mockups.  Every stage of the development process prior to the delivery of a minimum viable product (MVP) was completed.


## Problem Statement

These days, DIY home projects are very popular.  Walk-throughs can be found all over the internet for tasks such as making a bed-side table, painting rooms with interesting patterns, or even building a shed.

One of the main problems when it comes to these tasks is that the average person may not have the tools required readily available. It may also be exceptionally expensive for people to go buy those tools as well.  Spending the money to purchase the tool is unlikely when it is only needed for one specific project. DIY hobbyists require a service that enables them to rent the tools they require for a much lower fee than if they had to buy it themselves.

People who wish to complete home projects may also be limited by their lack of experience with the tools.  These people need to be provided with advice and video tutorials that will show them how to properly use the tools they wish to rent.

## Project Scope

This report outlines the design process for a web application for individuals who enjoy DIY projects but lack the tools to accomplish them.  The goal of the service is to provide a platform for people to rent tools for short-term periods to complete their tasks. It will also offer advice and tutorials for those who may require some help getting started.

The central purpose of the web application is to allow individuals in the London area to hire out tools for their projects.  The customer will be able to search through a selection of available tools, with the ability to sort by type, name, or project. Having found the desired tool, the customer will then check the calendar for its availability and then add it to the basket.  Upon check-out completion, the database will be updated to reflect the dates for which the tool is booked to prevent another customer from selecting those dates as well.

Customers may also view the blog containing weekly advice and subscribe to it if they wish. They may also submit queries to the customer support if they have any specific questions.

On the other side of the operation, employees may complete a range of tasks including managing the tool listings, uploading new blog posts, and responding to customer queries.

The success of the project would be measured by the delivery of the completed stages of the software development process prior to the creation of a prototype.  This would include requirements gathering, use-case analysis, object-oriented analysis and design models, and a system mockup. 

## Project Glossary

In order to be clear and consistent throughout the project, specific words and phrases were used.  These can be found in the glossary below.

\begin{table}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.8\textwidth]{TempImg/glossary.png}
      \caption{Project glossary containing key terms}
\label{conreq}
 \end{table}

## Gantt Chart
The Gantt charted shown below displays the project timeline followed by the team. It is divided into the four project phases outlined in the Unified Process: \textit{Inception, Elaboration, Construction and Transition}.

\begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.4\textwidth]{TempImg/gant.png}
      \caption{Gantt Chart Showing the Project Timeline}
 \end{figure}

## Project Management: SCRUM Embedded Unified Process

 The Unified Process or UP was developed in the 1990s and is a pragmatic and tested method for carrying out the development of a software system and was designed specifically for use with UML. Essentially, it is a process by which the \textit{who, what, and when} of a development project can be determined [2]. The three main principles of the UP are:

 \begin{itemize}
  \item The development process should be driven by use-cases and risk assessment
  \item The development process should emphasize a quality system architectural model 
  \item Software should be developed via step-wise completion of subprojects and continuous refinement through iteration
\end{itemize}


Within each iteration, five workflows are explicitly defined by the UP. These are Requirements, Analysis, Design, Implementation and Testing [2]. The broader project lifecycle is also covered in the UP and is made up of four distinct phases which are Inception, Elaboration, Construction and Transition. Within each of these phases, multiple iterations should take place to suit the project's needs. Figure 1.2 illustrates how all of the elements of the UP are tied together into a single project lifecycle. 

\begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.6\textwidth]{TempImg/UP.png}
      \caption{Outline of the Unified Process project lifecycle [2]}
 \end{figure}

SCRUM is a subset of Agile and is project management framework that grew out of the failures of previous models such as the Waterfall model. There are three empirical pillars that uphold any SCRUM project [3]. These are: 

\textbf{Transparency:} common standards are agreed upon within a team in order to avoid ambiguity.

\textbf{Inspection:} Users must inspect and update SCRUM artifacts throughout the development process.

\textbf{Adaptation:} Progress must be monitored by members of the SCRUM team and if the process has deviated to an unacceptable extent, the product(s) that resulted from that process must be reviewed and adapted.

These pillars underpin the SCRUM project lifecycle approach which involves:

\begin{enumerate}
  \item The SCRUM team meets in order to prioritize the artifacts in product Backlog. This could be a list of required features for a product.
  \item Before a Sprint begins, the team has a Sprint planning meeting to decide what work will be done during the Sprint.
  \item  The team does a Backlog refinement to confirm that the project is still on track before beginning the Sprint to ensure that work will not be wasted.
  \item  During the 2-4 week Sprint, the team has daily meetings which are short, lasting only 15 minutes or less. 
  \item At the end of each sprint, the team members present their work and have a Sprint Retrospective to analyze what could be improved during the next sprint. [4]
\end{enumerate}

\begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.8\textwidth]{TempImg/SCRUM.png}
      \caption{The SCRUM project lifecycle [4]}
 \end{figure}

For the DIY THS project, the team utilized both of these methodologies where they were suitable. The broader project lifecycle was shaped by the tenants of the Unified Process, while more day-to-day project management was derived from some useful features of SCRUM.  

The UP identifies that emphasizing system architecture and developing based on use-cases leads to successful products. This was integral to the development of the THS system. Given that the implementation was not carried out for the THS, the team had the opportunity to rigorously refine and identify essential use cases. From these use cases, object-oriented (OO) UML models were derived. After the essential system objectives were laid out through OO models, the architecture was modelled. Additionally, the THS team made use of the four phases of the Unified Process to help structure project progress which is illustrated in the Gantt chart in Section 1.6. 

While the team did not assign official SCRUM roles, certain useful aspects of SCRUM were adopted. Early in the project, the team developed a Backlog of the tasks that needed to be accomplished throughout the semester. Then, to fulfill these goals, the team worked in 1 week Sprints followed by Retrospectives to assess the challenges encountered in the previous week and plan the next Sprint. Additionally, transparency and standardized communication were essential for such a large group project and as such, a team glossary was used throughout. 

Both the UP and SCRUM outline the importance of iteration, which was the absolute core of the THS project. During the weekly Retrospectives, analysis of the previous weeks work was done by the team members and the project supervisor, which shed light on improvements to be made on the current work products. In many cases, several Sprints were used to refine a single work product. 

Overall, the project management was more of an adaptation of key tenants of both UP and SCRUM rather than an absolute adoption of all of their aspects. Ultimately, being able to utilize aspects of such models to suit the team’s needs resulted in very smooth project coordination and consistent progress throughout the semester.

\newpage 

# Requirements Gathering

## Overview

The first task for this project was to develop a list of requirements for the DIY Tool Hire Service.  To do so, the team began by organizing a meeting to discuss the scope of the project.  Once everyone came to a mutual understanding, the process of coming up with the requirements began.  During the meeting, the team reviewed the needs of the customer when using this type of service.  Each member then continued to develop requirements individually by researching existing web sites to find important functionalities as well as areas which may be improved.

This initial period of requirements development involved a lot of brainstorming.  The aim was to create a list of requirements that fully encompassed the website’s functionalities.  This would save time and effort further down the line, as making up for mistakes made during the requirement gathering period can become extremely costly [5].

The importance of the requirements gathering stage in the overall scope of the project cannot be overstated.  The requirements play a pivotal role in the progression of the project, directly influencing the development of use cases.  The use cases then go on to influence the classes and methods used, which in turn influence many of the future diagrams.  With that in mind, it was very important that the requirements gathering was done correctly. This is reflected in the significant portion of time that was allotted to develop the requirements, as seen in the Gantt chart in Section 1.6.


## Requirements

Although initially long and containing duplicates, the list of requirements was refined to fall in line with the scope of the project. These requirements were then broken down into subsections such as “Tool Hiring Process” and “Help & Advice” to aid in navigating the list and ensuring the user’s needs were accounted for. In Table 2.1, all of the functional and non-functional requirements have been assigned IDs and descriptions, as well as indications about the type of activity and the actors involved.  Additionally, every requirement was given a level of priority utilizing the MoSCoW system [6].

\begin{table}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.9\textwidth]{TempImg/req1.png}
 \end{table}

 \begin{table}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.9\textwidth]{TempImg/req2.png}
      \caption{MoSCoW prioritization of requirements for the THS system}
 \end{table}

## Domain Model Diagram

The domain model is used to represent the real-world actors and entities, as well as the relationships between them in the context of the problem space. It is a static model, in that it does not show any time or information flow. To develop the diagram, the actors and entities were derived from the requirements list, with nouns becoming entities and verbs becoming relationships.  They were then used to help reduce ambiguities that may arise during the design period as well as managing the complexity [7].  Additionally, the actors and entities represented some possible classes for the later stages of the development.

The domain model diagram was finalized over a sequence of iterations, with the latest version seen in Figure 2.1 below.  The actors, entities, and relationships between them are shown using UML notation. Once the entities were known, it was easier to construct the use cases more effectively.

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.99\textwidth]{TempImg/domain.png}
      \caption{Domain model diagram}
 \end{figure}

\newpage

# Use Cases 

## Overview

Having finished with the requirements gathering stage, the next task in the process involved developing and analysing a list of use cases.  Each use case represents some interaction taking place between an actor and the DIY Tool Hire Service [8].

The use case analysis stage is essential to the development of a proper software system.  It is vital that each of the requirements listed in Table 2.1 is accounted for when creating the use cases.  This was accomplished using an iterative process, during which the requirements were expanded and modified, and the use cases were adapted to support those changes.

During the use case analysis period, the team completed the use case list, use case diagram, use case specifications, and the use case/requirements matrix.  These tables and figures are found in the following subsections of this chapter.

## Use Case Listing

When brainstorming the potential list of use cases, it was necessary for the team to determine who the actors would be when interacting with the DIY Tool Hire Service.  The list of actors that was decided on based on the requirements came to: Customer, Admin, Credit Card Company, Notification Service, Customer Support, Database, and Delivery Service.  With the requirements and these actors in mind, a list of use cases was established. Over the course of several iterations, the list was adapted until the final list below was developed.

\begin{table}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.5\textwidth]{TempImg/UCListing.png}
      \caption{Use case listing}
 \end{table}

## Use Case Diagram

The use case listing from above was translated into a use case diagram.  The diagram presents the use cases in a more clearly illustrated manner. The team utilized the \textit{<<extend>>} relationship as a way to add optional behaviours to certain use cases, as well as the \textit{<<include>>} relationship to simplify larger use cases into more manageable parts [9].

\begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.9\textwidth]{TempImg/UCDiagram.png}
      \caption{Use case diagram}
 \end{figure}


## Use Case Specifications

Continuing the development process, the team took the use cases depicted above and provided much more detailed information for each including a description, the actors involved, pre- and post-conditions, as well as the main and alternative flows.  As the use case specifications were written, further alterations took place with the list of use cases.  The list of use cases was refined, and the specifications continuously updated throughout the project as more thought went into the behaviours of the actors.  The following specifications for the finalized list of use cases played a key role in the upcoming design period of the project [8].

\begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/UC1.png}
 \end{figure}

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/UC2.png}
 \end{figure}

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/UC3.png}
 \end{figure}

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/UC4.png}
 \end{figure}

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/UC5.png}
 \end{figure}

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/UC6.png}
 \end{figure}

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/UC7.png}
 \end{figure}

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/UC8.png}
 \end{figure}

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/UC9.png}
 \end{figure}

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/UC10.png}
 \end{figure}

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/UC11.png}
 \end{figure}

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/UC12.png}
 \end{figure}

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/UC13.png}
 \end{figure}

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/UC14.png}
 \end{figure}

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/UC15.png}
 \end{figure}

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/UC16.png}
 \end{figure}

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/UC17.png}
 \end{figure}

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/UC18.png}
 \end{figure}

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/UC19.png}
 \end{figure}

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/UC20.png}
 \end{figure}

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/UC21.png}
 \end{figure}

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/UC22.png}
 \end{figure}

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/UC23.png}
 \end{figure}

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/UC24.png}
 \end{figure}

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/UC25.png}
 \end{figure}

 \newpage


## Use Case/Requirements Matrix

The last task to accomplish during the use case analysis stage was to create a use case/requirements matrix.  This matrix, which displays the requirements on the left side and the use cases across the top, is intended to confirm that each of the requirements is being satisfied by one of the use cases and that each use case serves the purpose of meeting a requirement [4].  As seen below, the requirements and use cases established by the team satisfy these conditions. 

\begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.55\textwidth]{TempImg/UCRMatrix.png}
      \caption{Use case/Requirements matrix to describe how use cases fulfill system requirements}
 \end{figure}



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



\newpage# Application Mock-up

## Home Page 
\begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/home_screen.jpg}
      \caption{Home page for DIY THS}
 \end{figure}

 Presenting Do-It-Yourself Tool Hire! This is the home page of the site and the first one that a customer encounters when they visit.

## Create Account 
\begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/login_create_account.jpg}
      \caption{Create new account or log in page for DIY THS}
 \end{figure}

Before using the service, you can create a new account or log in if you are an exsisting user.
 

## New Customer Registration Page

\begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/open_account.jpg}
      \caption{Customer registration page for DIY THS}
 \end{figure}

 You can create a new account by filling in your account details, all fields are required and once filled out you can click open account to start hiring some tools. 

## Log-In Page

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/login_screen.jpg}
      \caption{Log-in page for DIY THS}
 \end{figure}

 To start using your new account enter the email address you used to create your account and your password. 

## Password Recovery 

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/forgot_password.jpg}
      \caption{Password recovery page for DIY THS}
 \end{figure}

 In the event that you forget your password you can click on the forgotten password link located on the home page. Type in the email address you used to register your account and click the send email button. You will be sent an email containing your password.  

## Manage Account 

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/manageAcc.png}
      \caption{Manage Account page for DIY THS}
 \end{figure}

Once logged in you also have the option of changing your account details by clicking on the My Account button. The form will be filled with your old account information and once you change a field you can click edit account to save your new account details. 

## Check Categories

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/cat.png}
      \caption{Check Categories for DIY THS}
 \end{figure}

 Under the checking categories we offer a different selection of tools for different tasks. As can be seen in the diagram below if you require a tool to aid in cleaning, the website offers many different cleaning tools which can be rented from floor scrubs to vacuum cleaners. 

 Once a tool has been selected you can view a short description of the item’s functionalities as well as the pricing plan for the item. You have the option of renting the item for one day, two days, a weekend or a full week. After deciding what option is best you can select your required start and end date.  

 \newpage

## Checks for Delivery Qualification

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/deliv.png}
      \caption{Checks for Delivery Qualification page for DIY THS}
 \end{figure}

 After selecting how much of the item you wish to rent you can click on check availability to see if it’s possible to deliver the item(s) to your postcode. To add the item to your checkout basket, click the orange basket icon next to ‘My account’. 

## Shopping Basket/Creates Order

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/basket.png}
      \caption{Shopping Basket/Creates Order page for DIY THS}
 \end{figure}

 After adding the item, you wish to rent to your basket you can review the final information about your order such as the required rental time and the final price including VAT. Click on ‘Checkout Safely’ to be taken to the Checkout and Payment page. 

## Checks Out

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/checkoutpic.png}
      \caption{Check out and payment details page for DIY THS}
 \end{figure}


On the payment page you will be able to fill out your debit/credit card details, billing address and shipping address. 

## Confirms Order & Updates Tool Availability & Track Order

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/confirm.png}
      \caption{Confirm order page for DIY THS}
 \end{figure}

After confirming your card details and it’s successful, you will be taken to the order confirmation page where you can track your order and view the expected delivery date. 

## Raises Query

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/query.png}
      \caption{Raises Query page for DIY THS}
 \end{figure}

 In the event that there is any additional information required. You can click on the help & support tab and fill out a form sending us a query about anything from delivery items to damaged equipment. 

## Reads Blog & Subscribes To Blog

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/readsblog.png}
      \caption{Blog page for DIY THS}
 \end{figure}

 You can find the blog under the help and support tab, where we release exciting new blogs about the latest tools, and tips and tricks on how to get the most out of your rentals! 

## Log Out

\begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/logout_screen.jpg}
      \caption{Log out page for DIY THS}
 \end{figure}

 After a customer has completed their session, they can log out of their account.

## Employee Login

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/adminlog.png}
      \caption{Employee Login page for DIY THS}
 \end{figure}

 All employees can login with their given account through the site’s employee portal. 

## Employee View & Manage Tools

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/managetool.png}
      \caption{Employee View for DIY THS}
 \end{figure}

 An employee has the ability to view all the tools currently on the site, as well as the ability to edit the description and to delete items. 

## Add Tools

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/addtool.png}
      \caption{Add Tools page for DIY THS}
 \end{figure}

 To add a new item, the employee must click on the add tools tab and fill out all the required information for the item before adding it.  

## Employee Add New Blog Entry

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/addblog.png}
      \caption{Add New Blog Entry page for DIY THS}
 \end{figure}

 Similarly, an employee can post a new blog by navigating to the add blog tab and filling out the form. 

## Employee Reply To Query

 \begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/qreply.png}
      \caption{Reply To Query page for DIY THS}
 \end{figure}

 The site also allows employees to reply to queries. The employee will see the name of the customer and their query and will have the ability to reply.  







\newpage

# Conclusion

In this chapter, an evaluation of the strategy utilized to design the THS will be provided, including a reflection on successes and challenges and some considerations for the future.

The team met on a weekly basis and, to increase the productivity, the team was divided into sub-groups to carry out varying work concurrently and efficiently. All documents were shared via OneDrive enabling everyone access to all stages of diagram iteration. During the weekly group discussion, the sub-group’s results were reviewed by the whole team with an open discussion in order to achieve high quality and consistency between all members. The weekly progress was monitored by the team’s advisor who gave feedback and advice on the tasks for the following week.

The development approach was based on strong requirements and use cases. The declaration of actors and their functionalities helped to create the classes and methods required for the Object-Oriented Analysis stage. As the team wanted to ensure that the flow of use cases was represented properly, many iterations of object oriented diagrams were made. (See Appendix). The current model is quite an advanced iteration, that would enable a development team to start implementation. The modular (object-oriented) nature of the design means further iteration of the classes and front-end development is possible without requiring major changes. This in-built design focused on short, simple iteration phases is in line with the tenants of the Unified Process.

Sustained communication throughout development and regular meetings comes across in the fluidity of the design, report and presentation. Both internal and external deadlines were met. These regular reviews and short sprints of individual work allowed us to overcome the challenge of synchronizing different backgrounds, knowledge bases and writing styles.

\begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.7\textwidth]{TempImg/conclusion.png}
      \caption{Successes and challenges for Group A.}
 \end{figure}

\textbf{Future Considerations}

A fully functional website design and implementation specification has been produced for the THS but there are some considerations which will need to be researched as the system is built and scaled:  

\textbf{Database Design:} Much of the data the system requires has been modelled in class variables. However, an entity-relationship diagram and data schema will need to be produced ahead of database development. This is crucial for the THS which is dependent on a database to function.  

\textbf{Concurrency:} One of the non-functional requirements was that the THS would allow 5000 concurrent users at any time. Therefore, consideration needs to be given to the implementation of this – for example building a multi-threaded application. 

\textbf{Front-end development:} A template should be built from the wire frame early on in the development of the system – to enable linking with the boundary classes, and to identify, early on, any iteration of the boundary classes/ interfaces needed.  

\textbf{Security:} This is crucial in a system with many users that stores sensitive information such as payment details and personal information. Consideration needs to be given to password and message encryption, firewalls and database security before the system can be used.  

\newpage

# References

\begin{enumerate}
  \item Jacobson, G. Booch, J. Rumbaugh, The Unified Software Development Process, Addison-Wesley, 1999.
  \item J. Arlow and I. Neustadt, UML and the Unified Process. London: Pearson Education, 2002.
  \item K. Schwaber and J. Sutherland, "The Scrum Guide", scrumguides.org, 2017. 
  \item "What's the Difference? Agile vs Scrum vs Waterfall vs Kanban", www.smartsheet.com, 2018. 
  \item F. Brooks, The Mythical Man Month, Addison-Wesley, 1975.
  \item A. Kline, Agile Development in the Real World, Apress, 2015.  
  \item S. Ambler, Agile Model-Driven Development with UML 2.0, Cambridge University Press, 2004.
  \item A. Cockburn, Writing Effective Use Cases, the Crystal Collection for Software Professionals, Addison-Wesley, 2000.
  \item R. Miles & K.Hamilton, Learning UML 2.0, O’Reilly, 2006.
  \item A. Kalmback (2015). ‘Entity-Boundary-Interactor; A modern application architecture’. readthedocs.io [Online]. Available: http://ebi.readthedocs.io/en/latest/
  \item Whitten, L. Bentley and K. Dittman, Systems analysis and design methods. Boston, Mass.: Irwin/McGraw-Hill, 1998.
  \item E. Gamma, R. Helm, R. Johnson and J. Vlissides, Design patterns. Boston, Mass.: Addison-Wesley, 2016.
  \item "Three-tier architectures", ibm.com, 2018.
  \item “Using a Three-Tier Architecture Model", msdn.microsoft.com, 2018. 
\end{enumerate}