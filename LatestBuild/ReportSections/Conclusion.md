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