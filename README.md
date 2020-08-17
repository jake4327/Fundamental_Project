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
### Mission statement
> To build a world where people pay for whats theres.
### Idea
> A weight system to measure liquid in bottles.
### Application
> To be used in hospitality sector, in bars to produce an accurate live stock count

## Speicfication link
> How is application a CRUD application?

### Enter new spirit
* C - A new brand of alcohol 
* R - Bottled spirt information
* U - Change bottled spirt information
* D - Delete bottled spirt

### Pour Spirt
* C - New bottle
* R - Current bottle weight
* U - Pour spirit
* D - Delete current weight

### Bar session
* C - 
* R -
* U - 
* D - 

## Planning

### Kanban board 

Why use a kanban board 
How did you use it to maximise effiency
What sprints did you use?
Why did you pick these sprints - because it made me move towards the MVP? 

![](images/kanban_board_one.png)

### Planning breakdown

This section will focus on how the proposed project will reach it minimum MVP on each relase release the versions
* version 1
> Minimus Viable Product 
> Have 1 C, R,U and D happening.
> Have SIMPLE till system - One button with vodka on it, hard code price and weight
> Focus on pour session - One vodka poured -> ran through till -> bottle put back on scale


* version 2
> Create second CRUD process running
> Add one more spirit to the bar Gin
> Focus on bar session - one bar opens -> allows bar seesion to run -> closes produces report

* version 3
> Add sever

* version 4 
> Create different brands of alcohol 
> Create user interface company interface for signing up to company
> Create a system 

##Design

### UML

#### Database Design 
![](images/pour_spirit-Database%20Model.png)

#### Bar Session
![](images/pour_spirit-Bar%20session.png)

#### Pour Bottle 
![](images/pour_spirit-Pour%20Bottle.png)


### Website view

#### Enter new Bottle
![](images/Enter_Bottle_Page.png)

#### Till System
![](images/till_system_complete.png)

## Risk Assessment
![](images/moscow_risk_assessment.jpg)

### Technical risk assessment

|Risk_ID                  |Description                                                       |Assessment                                   |Risk  |Impact |Responsiblity |Current Mitigration      |Proposed Mitigration|Respone|Tolorance|
|-------------------------|------------------------------------------------------------------|---------------------------------------------|------|-------|--------------|-------------------------|--------------------|-------|---------|
|0_0001                   |Java test not complete                                            |                                             |      |       |              |                         |                    |       |         |
|0_0002                   |README.md not complete                                            |                                             |low   |low    |low           |Monitor readme           |                    |       |         |
|0_0003                   |Unit test not evaluating function correctly                       |Function will not produced desired output    |high  |high   |              |Design unit tests        |                    |       |         |
|0_0004                   |Integration test not evaluation combination of function correctly |Combined functions don't pass data correctly |hight |high   |              |Design integration tests |                    |       |         |
|0_0005                   |Create function fails                                             |                                             |      |       |              |                         |                    |       |         |
|0_0006                   |Read function fails                                               |                                             |      |       |              |                         |                    |       |         |
|0_0007                   |Update function fails                                             |                                             |      |       |              |                         |                    |       |         |
|0_0008                   |Delete function fails                                             |                                             |      |       |              |                         |                    |       |         |
|0_0009                   |Loss of internet                                                  |                                             |      |       |              |                         |                    |       |         |
|0_0010                   |Damage to internet infrastructure                                 |                                             |      |       |              |                         |                    |       |         |

### Personal Risk assessment


|Description                 |Assessment                                        |Risk  |Impact |Responsiblity |Current Mitigration                                                                    |Proposed Mitigration            |Respone|Tolorance|
|----------------------------|--------------------------------------------------|------|-------|--------------|---------------------------------------------------------------------------------------|--------------------------------|-------|---------|
|Self state                  |My own state of mind to continue with the project |low   |high   |Jake Stone    |Eat, sleep, excercise, in communication with QA team                                   |                                |       |         |
|Not understanding technology|                                                  |high  |high   |Jake Stone    |Notes, pictures, videos, when something is not understood ask team members and Mentors |Getting mentor to record videos |       |         |

### MoSCoW

#### Must


#### Should

#### Clould

#### Would 
