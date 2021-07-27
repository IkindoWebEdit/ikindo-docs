

# Test plan

 

## 1.   Introduction

### 1.1 Purpose

The purpose of the Test Plan is to gather all of the information necessary to plan and control the testing.

It describes the approach to testing the software.

This Test Plan supports the following objectives:

-       Identifies the items that should be targeted by the tests.

-       Identifies the motivation and ideas behind the test areas.

-       Outlines the testing approach that will be used.


 

### 1.2 Scope

The areas of tests that are considered in document are:

* Selenium for everything programmed in django




 

### 1.3 Intended Audience

This document will only be used internally.

 

### 1.4 Document Terminology and Acronyms

- **SRS**      Software Requirements Specification

- **SAD**      Software Architecture Document

- **n/a**      not applicable

- **tbd**      to be determined

 

### 1.5 References

| Reference        |

| ------------- |

| [Blog](https://ikindowebedit.wordpress.com/) |

| [SRS](https://github.com/IkindoWebEdit/ikindo-docs/blob/main/SRS.pdf) |

| [SAD](https://github.com/IkindoWebEdit/ikindo-docs/blob/main/SAD.pdf) |

 

## 2.   Evaluation Mission and Test Motivation

### 2.1 Background

By testing our project, we basically make sure that everything works while programming. Also we can make sure that no funcionallity breaks, while changing the source code or adding new features. By integrating testing in our development process, we also make sure that no versions with bugs get commited.

### 2.2 Evaluation Mission

Our mission is to deliver a product with 100% functionality. Testing helps us to provide that, because we can spot errors and parts that dont work how they should before deploying our project to the customer.

### 2.3 Test Motivators

Our testing is motivated by

- use cases

- functional requirements

 

## 3.   Target Test Items

* Administrator login
* Django functionality in genereal

## 4.   Outline of Planned Tests

### 4.1 Outline of Test Inclusions

* FeatureFiles

* Selenium

 

### 4.2 Outline of Other Candidates for Potential Inclusion

n/a

### 4.3 Outline of Test Exclusions

n/a

 

## 5.   Test Approach

### 5.1 Testing Techniques and Types

Because most of our script is interactive with edit functionality we aren't really aware of testing it. The correctnes of this will be checked through code analysis only.
What we can test are functionality of everything that is written in django like the logging, switching sites, administration of rights etc.. For those we will use functional tests.
Those Test will open a browser instance, pressing buttons, filling out text areas etc..  

#### 5.1.1     Function and Database Integrity Testing

|||

|---|---|

|Technique Objective|Every django function gets evaluated correctly|

|Technique|Simple function Tests|

|Required Tools|Selenium|

|Success Criteria|successful scenarios, all tests will pass, no strange behaviour will occur|

|Special Consideration|-|

 

#### 5.1.2     Unit Testing

n/a

#### 5.1.3     Business Cycle Testing

n/a

 

#### 5.1.4     User Interface Testing

|||

|---|---|

|Technique Objective|Every input in the website will be elaborated correctly||

|Technique|Integration tests on the rendered UI|

|Required Tools|Selenbium |

|Success Criteria|successful scenarios, all tests will pass, no strange behaviour will occur|

|Special Consideration|-|

 

#### 5.1.5     Performance Profiling

n/a

 

#### 5.1.6     Load Testing

n/a

 

#### 5.1.7     Stress Testing

n/a

#### 5.1.8     Volume Testing

n/a

 

#### 5.1.9     Security and Access Control Testing

|||

|---|---|

|Technique Objective|Different inputs will be checked ||

|Technique|Integration tests on the rendered UI|

|Required Tools|Selenbium |

|Success Criteria|amdin loginj should be accepted, wrong input declined|

|Special Consideration|-|

 

#### 5.1.10    Failover and Recovery Testing

n/a

 

#### 5.1.11    Configuration Testing

n/a

 

#### 5.1.12    Installation Testing

 

## 6.   Entry and Exit Criteria

### 6.1 Test Plan

**n/a**

#### 6.1.1     Test Plan Entry Criteria

On to the correct webpage 

#### 6.1.2     Test Plan Exit Criteria

When all tests pass without throwing an exception.

#### 6.1.3 Suspension and Resumption Criteria

Wrong inputs, wrong buttons pressed to the wrong time 

 

## 7.   Deliverables

### 7.1 Test Evaluation Summaries

n/a

 

### 7.2 Reporting on Test Coverage

n/a


### 7.3 Perceived Quality Reports

n/a

 

### 7.4 Incident Logs and Change Requests

n/a

 

### 7.5 Smoke Test Suite and Supporting Test Scripts

n/a

 

### 7.6 Additional Work Products

n/a

 

#### 7.6.1     Detailed Test Results

n/a

 

#### 7.6.2     Additional Automated Functional Test Scripts

n/a

 

#### 7.6.3     Test Guidelines

n/a

 

#### 7.6.4     Traceability Matrices

n/a

 

## 8.   Testing Workflow

Test will be run in the build process or manually when editing the django files.
 

## 9.   Environmental Needs

Automated execution on build

### 9.1 Base System Hardware

n/a
 

### 9.2 Base Software Elements in the Test Environment

The following base software elements are required in the test environment for this Test Plan.

 

| Software Element Name |  Type and Other Notes                        |

|-----------------------|----------------------------------------------|

| Python 		| > 3.0		                               |

| Selenium              | > 3.0		                               |



 

 

### 9.3 Productivity and Support Tools

n/a



### 9.4 Test Environment Configurations

n/a

 

## 10.  Responsibilities, Staffing, and Training Needs

### 10.1       People and Roles

This table shows the team-roles for testing.

|Role|Minimum Resources Recommended(number of full-time roles allocated)|Specific Responsibilities or Comments|

|---|---|---|

|Test Manager|1|Manages the testing.  Responsibilities:  test-planning and coordination |

|Test Designer|1|Defines the technical approach to the test-implementation.  Responsibilities: defining test approach and test automation architecture, verify test techniques|

|Tester|1|Implements and executes the tests. Responsibilities: implementing and executing tests, logging results and analyzing test failures|

 

### 10.2       Staffing and Training Needs

n/a

## 11.  Iteration Milestones

 

| Milestone | Planned Start Date | Actual Start Date | Planned End Date | Actual End Date |

|---|---|---|---|---|

| Implemented tests | n/a |  n/a  |  n/a  |  n/a |

| 20% coverage | n/a |  n/a  |  n/a  |  n/a  |

 

 

## 12.  Risks, Dependencies, Assumptions, and Constraints

| Risk | Mitigation Strategy   | Contingency (Risk is realized) |

|---|---|---|

| Untestable features in <br/>the framework | Cannot be avoided | Try to test it with integration tests |

| Some functionallities are not <br/>covered | Carefully design tests | Add more tests |

| Technical Difficulties for customers | Try to help remote | Try it out on different browsers before deploying |

## 13. Management Process and Procedures

<a href = https://ikindowebedit.wordpress.com/2021/05/25/s2-week-7-metrics/>Link to our Metrics</a>

 
