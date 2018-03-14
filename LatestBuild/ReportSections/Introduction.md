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

The iterative nature of the USDP resulted in multiple evolutions at every step in the process.  While each aspect of development – from the requirements gathering and use cases to the object-oriented diagrams – underwent several iterations, only the final iterations have been included within the report.  All of the diagrams found in this report were completed in Unified Modeling Language (UML) format, the industry standard.

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
The Gantt charted shown below displays the project timeline followed by the team.

\begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.4\textwidth]{TempImg/gant.png}
      \caption{Gantt Chart Showing the Project Timeline}
 \end{figure}

## Project Management: SCRUM Embedded Unified Process

 The Unified Process or UP was developed in the 1990s and is a pragmatic and tested method for carrying out the development of a software system and was designed specifically for use with UML. Essentially, it is a process by which the who, what, and when of a development can be determined. [2] The three main principles of the UP are:

 \begin{itemize}
  \item The development process should be driven by use-cases and risk assessment
  \item Components related to the Warehouse management. It manages which tools are available and in which quantity.
  \item The development process should emphasize a quality system architectural model 
  \item Software should be developed via step-wise completion of subprojects and continuous refinement through iteration
\end{itemize}


Within each iteration, five workflows are explicitly defined by the UP. These are requirements, analysis, design, implementation and testing. (UP book) The broader project lifecycle is also covered in the UP and is made up of four distinct phases which are inception, elaboration, construction and transition. Within each of these phases, multiple iterations should take place to suit the projects needs. Figure 1.2 illustrates how all of the elements of the UP are tied together into a single project lifecycle. 

\begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.6\textwidth]{TempImg/UP.png}
      \caption{Outline of the Unified Process project lifecycle [2]}
 \end{figure}

SCRUM is a subset of Agile and is project management framework that grew out of the failures of previous models such as the Waterfall model. There are three empirical pillars that uphold any SCRUM project. [3] These are: 

\textbf{Transparency:} common standards are agreed upon within a team in order to avoid ambiguity.

\textbf{Inspection:} Users must inspect and update SCRUM artifacts throughout the development process.

\textbf{Adaptation:} Progress must be monitored by members of the SCRUM team and if the process has deviated to an unacceptable extent, the product(s) that resulted from that process must be reviewed and adapted.

These pillars underpin the SCRUM project lifecycle approach which involves:

\begin{enumerate}
  \item The Scrum team meets in order to prioritize the artifacts in product backlog. This could be a list of required features for a product.
  \item Before a Sprint begins, the team has a Sprint planning meeting to decide what work will be done during the sprint.
  \item  The team does a backlog refinement to confirm that the project is still on track before beginning the Sprint to ensure that work will not be wasted.
  \item  During the 2-4 week Sprint, the team has daily meetings which are short, lasting only 15 minutes or less. 
  \item At the end of each sprint, the team members present their work and have a Sprint Retrospective to analyze what could be improved during the next sprint. [4]
\end{enumerate}

\begin{figure}[H]
      \centering
      \includegraphics[trim = 0 0 0 0, clip, width=0.8\textwidth]{TempImg/SCRUM.png}
      \caption{The SCRUM project lifecycle [4]}
 \end{figure}

For the DIY THS project, the team utilized both of these methodologies where they were suitable. The broader project lifecycle was shaped by the tenants of the Unified process, while more day-to-day project management was derived from some useful features of SCRUM.  

The UP identifies that emphasizing system architecture and developing based on use-cases leads to successful products. This was integral to the development of the THS system. Given that the implementation was not carried out for the THS, the team had the opportunity to rigorously refine and identify essential use cases. From these use-cases, object oriented (OO) UML models were derived. After the essential system objectives were laid out through OO models, the architecture was modeled. Additionally, the THS team made use of the four phases of the Unified Process to help structure project progress which is illustrated in the Gantt chart in Section 1.6. 

While the team did not assign official SCRUM roles, certain useful aspects of SCRUM were adopted. Early in the project, the team developed a backlog of the tasks that needed to be accomplished throughout the semester. Then, to fulfill these goals, the team worked in 1 week Sprints followed by Retrospectives to assess the challenges encountered in the previous week and plan the next Sprint. Additionally, transparency and standardized communication was essential for such a large group project and as such, a team glossary was used throughout. 

Both the UP and SCRUM outline the importance of iteration, which was the absolute core of the THS project. During the weekly Retrospectives, analysis of the previous weeks work was done by the team members and the project supervisor, which shed light on improvements to be made on the current work products. In many cases, several Sprints were used to refine a single work product. 

Overall, the project management was more of an adaptation of key tenants of both UP and SCRUM rather than an absolute adoption of all of their aspects. Ultimately, being able to utilize aspects of such models to suit the team’s needs resulted in very smooth project coordination and consistent progress throughout the semester.

