# MyWebServer-Test-Analysis
Prepared by: _John Doe (Test-Lead)_
Version: 1.0.0
Project name: MyWebServer-Test-Analysis

### Introduction

This report contains a detailed test analysis for the web server application MyWebServer.


###  Table of contents
* [Test Strategy](#Test Strategy)
* [Test Plan](#Test Plan)
* [Test Cases](#Test Cases)
* [Test Report](#Test Report)

___

## Test Strategy
####   Contents
* [Test Levels](#Test Levels)
* [Roles and Responsibilities](#Roles and Responsibilities)
* [Environment Requirements](#Environment Requirements)
* [Testing Tools](#Testing Tools)
* [Risks and Mitigation](#Risks and Mitigation)
* [Test Schedule](#Test Schedule)
* [Regression test approach](#Regression test approach)
* [Test Groups](#Test Groups)
* [Test Priorities](#Test Priorities)
* [Test Status Collections and Reporting](#Test Status Collections and Reporting)
* [Test Records Maintenance](#Test Records Maintenance)
* [Requirements traceability matrix](#Requirements traceability matrix)
* [Test Summary](#Test Summary)

### Related documents
| #Ref | Document                  |
|------|---------------------------|
| 01   | WebServerRequirements.pdf |

### Glossary
| Term | Definition               |
|------|--------------------------|
| JIRA | Incident management tool |

### Roles
**Test lead**: Responsible for testing and for creating this documentation
**Product owener:** Expert in the bussiness logic for Software Development Company (SDC).

### Purpose
This document is a high level presentation of the test approach to be undertaken in relation to the MyWebServer. Once formally accepted by the product owner at Software Development Company (SDC), this document will be used as a reference the test lead to develop a Test Plan with details of test activities resourcing and schedules.

This Test Strategy will underpin all subsequent testing activities and as such is presented for product owner at SDC for sign off as approval of the proposed approach.
  
### Project Overview
The project consists of a pre-developed web server called MyWebServer. 

### Testing objectives
The objective with the tests is to deliver a easy to deploy, well tested, open source, web server that support multiple platforms.

The requirements that the product shall provide are the following:
Req 1. The web server should be responsive under high load.
Req 2. The web server must follow minimum requirements for HTTP 1.1
Req 3. The web server must work on Linux, Mac, Windows*.
Req 4. The source code should be released under GPL-2.0.
Req 5. The access log should be viewable from a text editor.
* XP, Vista, 7, 8, 10, Server 2008

### Test levels
Test levels are used to split testing phase into logical phases and set clear boundaries for each level of testing. In this project we will test the following three levels:
- Component testing/Unit testing
- System testing
- User Acceptance Testing (UAT)

**Component testing** relates to the testing of individual software components i.e. unittests created by developers. In the MyWebServer code base there are already pre-existing unittests that coveres all the component testing we need.

**System testing** is done to ensure that the whole system works when integrated.  

**User Acceptance Testing** is done togheter with the product owner to establish confidence in the system. The product owner will also help to create test cases with help from the expert bussiness logic knowledge that he pocess.

### Test types
This table describes all the types of testing that shall be performed for the different levels.

| Test Types          | Component Testing | System Testing | UAT |
|---------------------|-------------------|----------------|-----|
| Static test         | Yes               |                |     |
| Functional test     | Yes               | Yes            | Yes |
| Non-functional test |                   | Yes            | Yes |
| Security test       |                   |                | Yes |
| Negative test       | Yes               | Yes            |     |

All component tests and some of the system tests will be automated.

### Pass/Fail criteria
Test Scripts will be developed as a part of every test case. The test scripts will contain test steps, expected results, pass criteria and fail criteria. 
Broadly speaking, deviation from what is written in a functional / technical specification will be considered a defect. A defect might not always result in failure.
Where a defect is identified, a defect record will be raised for each deviation between the test result and the expected result recorded in the test scripts, which are in turn based on the relevant functional / technical specification. 
If the incident is investigated and found not to be an error, the defect will be assigned back to the test lead for closure. 
If the incident is found to be a real error, it will be prioritised based on input from the relevant developers and product owner.

### Entry Criteria
Since the product is already created and we have the requirements in the document WebServerRequirements(#Ref-01) we can start testing immediately.

### Exit Criteria
These are the minimum acceptable conditions before promoting the MyWebServer solution to a live production environment:

- There are no outstanding high priority issues
- All Test Cases have been successfully executed
- Test coverage of 80% has been completed

## 4. Project Conditions
### Assumptions
The following assumptions have been made in preparing this test strategy:
- The test environment will be available at the start of the testing period.
- Technical resources will be available to provide support for the resolution of project issues/defects.
- The requirements in WebServerRequirement(#Ref-01) are not to be changed.

## 5. Proposed testing approach
### Test iterations and deadlines
Tests iterations will be done in two iterations, since the product is already developed we need one iteration to identify errors and another to rerun the tests after issues are fixed. The test plan will prioritise testing and include dates.

### Defect Management
The detection, management and resolution of defects will be properly created and progressed using JIRA.
All defects must be assessed to determine a severity level as described in the table below.

| Severity | Severity Description               |
|----------|------------------------------------|
| High     | MyWebServer crashes                |
| Medium   | Major system component is unusable |
| Low      | Incorrect or incomplete logic      |


### Test Environment
The following test environments will be used:

| Type      | Test environment | Description                                                                                                                                |
|-----------|------------------|--------------------------------------------------------------------------------------------------------------------------------------------|
| Automated | SauceLabs        | Cloud service that provides images for all different operating systems that we need.  Linux, Mac, Windows XP, Vista, 7, 8, 10, Server 2008 |
| Manual    | OSX              | MacBook Pro with OSX and Chrome webbrowser                                                                                                 | 

##### Test Summary


## Test Plan

## Test Cases

## Test Report

