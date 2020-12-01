# msem-sw.arch-c4-model-assignment

Andreas Heil | aheil | Yesterday, 15:01
## Appointment on the 30th of November
Dear Students,

Today, I will not be able to do a lecture in person as we have our project week.

Eventually, I would like to ask you to use the time as project time to work on the assignment below. However, you are free to assign your time individually. Please be aware, the assignment has to be submitted by next Monday (= Sunday, 11:59 pm). Please work through the assignment in your existing groups.

As mentioned last week, this assignment will substitute for the midterm exam.

The assignment will consist of creating C4 model diagrams using the toolset introduced last week.

All the links to the tools will be provided below:

## Task 1: Tooling

1. IF not done so far, make sure to be familiar with the C4 model. Please study the information provided here: https://c4model.com/

2. Watch the video provided here to repeat the information about the C4 model: https://www.youtube.com/watch?v=x2-rSnhpw0g&feature=emb_logo

3. To create the diagrams, I recommend Visual Studio Code: https://code.visualstudio.com/.

You can use any other (text-based) editor if you want. However, with Visual Studio Code you will gain the complete toolchain. For the evaluation of the assignment, the editor is not relevant.

4. Make sure you install PlantUML from here https://plantuml.com/. Follow the installation instruction carefully, especially, as you need to install GraphViz as a layout engine during this process.

5. If you are using Visual Studio Code, please make sure you install the PlantUML extension from https://marketplace.visualstudio.com/items?itemName=jebbs.plantuml as well.

6. After installation, please make yourself familiar with the PlantUML syntax and usage using the quick start guide at https://plantuml.com/starting (it is quick indeed).

7. Read through the C4-PlantUML extension introduction here: https://github.com/plantuml-stdlib/C4-PlantUML.Make sure you can use the extension with your installation.

8. In case you are using Visual Studio code, make sure you setup your editor to use the corresponding snippet: https://github.com/plantuml-stdlib/C4-PlantUML#snippets-for-visual-studio-code.

9. In case you have issues with any of the tools, you can create the diagrams using the online editor: http://www.plantuml.com/plantuml/uml/SyfFKj2rKt3CoKnELR1Io4ZDoSa70000 (also works with the extension).

 

## Task 2: Architecture models

Based on the following description, please create three diagrams (level 1, level 2, and level 3).

Regarding the technology and design choices made by your team for level 2 and 3 diagrams, you are free of choice, based on your experience in the team. Consider carefully, which systems are part of your diagrams and which are not.

Scenario:

The overall system considered, is a electronic health record application, developed by your team. Users of the system are internal employees of the health insurance agencies. The users access a web application, written in Java and Spring Boot. Interaction takes place via HTTPS. The web application provides static content as well as a single page application (SPA) written in Microsoft Blazor. This SPA in turn does provide the overall functionality in a web browser. The users do use the SPA via HTTPS. The SPA does use an API application based on Go in Docker containers. Due to their number, the containers are managed by Kubernetes. The Kubernetes cluster is maintained by your centra IT department. The API application provides the overall accounting functionality by providing a synchronous JSON/HTTPS based API. This functionality is based on an SAP R/3 System connected asynchronously using RFC (Remote Function Call). The SAP System is a system of the particular health insurance, using a dedicated e-mail server not hosted by your organization. This Microsoft Exchange Server does send out a daily report to the customers. External auditors access the reporting functionality of the SAP system using a data warehouse system based on a DB2 system to the SAP system using a proprietary SQL implementation.

## Submission:
Please submit your work (three .puml files) as a single ZIP file in ILIAS at the assignment section. 

If you have any questions related to the assignment, please comment on this message.


Kind regards,
A. Heil
