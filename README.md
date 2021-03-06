 # Fundamental_Project
QA SFIA1 project

Introduction

# Live Bar Count

![](images/Beer_weight_design.png)

## Contents
- [Introduction](#Introduction)
- [Design](#Design)
- [Architecture](#Architecture)
- [Risk Assessment](#Risk%20Assessment)

## Introduction

### Idea
> A weight system to measure liquid in bottles.
### Application
> To be used in hospitality sector, in bars to produce an accurate live stock count

## Planning

### Kanban board 

The Kanban board is used to organise a project. The tasks are set into Epics which is a list of the main goals to achieve. These main goals are accompanied by stories and tasks which are the aims and objectives of the goal. The aims are smaller tasks that need to be completed to achieve the goals and objective are the most granular type of task.

Using a Kanban board aims to maximise efficiency and to monitor work progression. The Atlassian software being used for this project is filled with functionality to measure the productivity of my development. Monitoring work like this allows for the Business operations team to make decisions about the product, such as when they believe the product will be ready to realise.

The second reason people use a kanban board, through Jira is to maximise efficiency. Using a monitoring system like this is excellent because it helps focus people on the essential tasks and the progression of the project can be viewed which motivates people to complete the task.

The final and most important thing the Jira board does is help the project move towards the MPV, which is essential to the project. Having the minimum viable product allows the business to sell its product and pay the developers while they work on improving and adding new features.

![](images/kanban_board_one.png)

### Planning breakdown

This section will focus on how the proposed project will reach it minimum MVP on each relase release the versions.
The versions will be dictated from a MoSCoW product point of view:
* MUST have:
  * Minimus Viable Product
  * Have 1 C, R,U and D happening.
  * Have back end running on Google vm

* SHOULD have:
  * A second CRUD process running
  * Impliment testing and see if the testing goes into 

* COULD have:
  * Create waste, bar, company class 
  * Design front end and 
  * Allow access to front end on the google VM

* WON'T have: 
  * Scaling of Virtual Machines

### Continuous Integration Pipeline 

The CI pipeline layouts how the project works with its different technologies. The different technologies are 
split into three sections the Developers section, the DevOps section and finally the Deployment section.

The first section is the Developers section, this section is where the code is planned and written. The planning 
of the project is done on the Jira board as discussed above and the code is written in Java and both of these       
technologies keep the working code base up to date by pushing and pulling to/from git hub, respectively.

The next section is the DevOps section, in this section we see CircleCI building the code from Maven.
CircleCI is a continuous integration pipeline that allows for tasks to be done every time something is pushed to the repository on GitHub. This allows the application to constantly being checked online and if it goes offline then it
is clear as to why it is offline. When CircleCI installs maven and runs the application via Maven, it sends either an error report to the Gmail account or continues to run.

The final part of the CI pipeline is the deployment, there are two google cloud boxes and these show that CircleCI 
connects with the virtual machine then runs the application on the virtual machine.
![](images/CI_pipeline.png)

## Design

### UML

#### Database Design 

This model shows the relationships between the entities within the application at the current state of the application. There is an Alcohol brand entity and a Bottles entity, the diagram shows that you can have many, 
bottles to one alcohol brand and only one alcohol brand for a bottle.

![](database_design/ERD_Chen_conceptual_model.png)

#### Bar Session

Diagram showing flow chart of Bar session.

![](images/pour_spirit-Bar%20session.png)

#### Pour Bottle 

Diagram showing flow chart of the Pour session.

![](images/pour_spirit-Pour%20Bottle.png)

### Class Diagram

Class diagram shoing how classes within the applicationa are interaction with each other.

![](images/UML.png)

### Website view

#### Enter new Bottle

A simple vision on how the html page for entering a new bottle would look.

![](images/Enter_Bottle_Page.png)

#### Till System

A simple vision on how the html page for the till system would look.
![](images/till_system_complete.png)

### Technical risk assessment

|Description                      |Assessment                                                            |Risk        |Impact|Responsiblity                  |Current Mitigration|Proposed Mitigration                                                         |Respone                                                         |Tolorance|
|---------------------------------|----------------------------------------------------------------------|------------|------|-------------------------------|-------------------|-----------------------------------------------------------------------------|----------------------------------------------------------------|---------|
|Damage to internet infrastructure|If the virtual machine on google goes down                            |high        |high  |Google cloud services, CircleCI|none               |Use a different cloud provider                                               |Poor - application will still be down when Google Cloud is down.|high     |
|Sensitive data exposure          |Alocohol brands and the product lines they sell are public information|no existent |none  |Jake Stone                     |None               |When business data is being handeled another risk assessment will be complete|                                                                |high     |


### Personal Risk assessment

|Description                                                     |Assessment                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |Risk  |Impact |Responsiblity        |Current Mitigration                                                                            |Proposed Mitigration                                                                                                                       |Respone                                                                   |Tolorance                                                                                                   |
|----------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------|-------|---------------------|-----------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------|
|Time to learn.                                                  |Time to learn to learnt he new technologies has been minimal. The amount of time spent on java, springboot, circleCi, HTML, CSS, database design/database query language etc. Has been minimal.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |high  |high   |Jake Stone           |Notes, pictures, videos, when something is not understood ask team members and Teachers at QA. |Only adding code/application that is understood so that if something breaks it can be easily fixed.                                        |weak - how to measure understanding of every function within application? |low - This reposnse is a better response than doing nothing and implimenting things that are not understood.|
|Scope of work is poorly specified                               |When given the mark scheme, I was told I need to develop an application that needed to have C(reate)R(ead)U(pdate)D(elete) functionality. The rest of the scope was defined by myself.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |low   |high   |Jake Stone/QA mentors|Design application with good planning with Jira board                                          |To have different versions of the project to scale back the scope quickly if have went too far with the scope.                             |Good                                                                      |High                                                                                                        |
|Unexpected changes and uncontrolled growth to a project’s scope.|If my project gets taken on by other people interested in developing it                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |low   |low    |Jake Stone           |Ignore other developers if they want to push to my project                                     |Put GitHub project on private so nobody can fork it and add the markers as contributors so nobody can fork my project and develop it for me|Good                                                                      |High                                                                                                        |


