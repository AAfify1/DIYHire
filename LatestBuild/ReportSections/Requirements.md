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

