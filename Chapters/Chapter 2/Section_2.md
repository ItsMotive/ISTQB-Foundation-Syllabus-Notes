<details>
  <summary>Table of Contents</summary>
  <ul>
    <li><a href="/README.md">Home</a></li>
    <li><a href="Chapter_2_Home.md">Chapter Home</a></li>
    <li><a href="Section_1.md">Section 1</a></li>
    <li><a href="Section_2.md">Section 2</a></li>
    <li><a href="Section_3.md">Section 3</
  </ul>
</details>

## Section Guide

- [Test Levels and Test Types](Section_2.md#22)
- [(K2) Distinguish the different test levels](Section_2.md#221)
- [(K2) Distinguish the different test types](Section_2.md#222)
- [(K2) Distinguish confirmation testing from regression testing](Section_2.md#223)

<a id=22></a>

## Test Levels and Test Types

- **Test Types**

  - Groups of test activies related to specific quality characteristics
    - Most of these test activities can be performed at every test level

- **Test Levels**

  - Groups of Test Activities that are organized and mmanaged together
  - Each level is an instance of the test process, performed in relation to software at a software development stage
    - This includes individual components to a complete system or system of systems
  - In **Sequential SDLC Model**
    - Test levels are often designed to be part of Exit Criteria of one level and Entry Criteria of another.
  - In **Iterative SDLC Model**
    - May not apply

  <a id = 221></a>

  ## (2.2.1) Test Levels

  - To avoid overlapping of test activities, Test Levels are distinguished by the following list of attributes:

    - Test Object
    - Test Objectives
    - Test Basis
    - Defects and Failure
    - Approach and Responsibilities

  - Here are 5 Test Levels:
    - **Component Testing** (Unit Testing)
      - Often requires Test Harnesses or Unit Test Frameworks
      - Normally performed by Developers in their Development Environmment
    - **Component Integration Testing** (Unit Integration Test)
      - Testing interfaces and interactions between components
      - Heavily dependent on the Integration Strategy Approaches:
        - Bottom-Up
        - Top-Down
        - Big-Bang
    - **System Testing**
    - **System Integration Testing**
    - **Acceptance Testing**

## Section Guide

- [(K2) Distinguish the different test levels](#221)
- [(K2) Distinguish the different test types](#222)
- [(K2) Distinguish confirmation testing from regression testing](#223)

<a id=22></a>

## (2.2) Test Levels and Test Types

- **Test Levels** are groups of Test Activities that are organized and managed together
- Each Test Level is an instance of the test process, performed in relation to software at a stage of development, from individual components to complete systems

- In **Sequential SDLC Model**
  - Often defined as Exit Criteria for one level and Entry Criteria for another
- In **Iterative SDLC Model**
  - May not apply
  - Development Activities may span through multiple tests
  - Test levels may overlap in time
- **Test Types** are groups of test activities related to specific quality characteristics

  - Most test activities can be performed at every test level

  ## (2.2.1) Test Levels

  - To avoid overlapping of Test Activities, Test Levels are distinguished by a list of attributes:

    - Test Object
    - Test Objectives
    - Test Basis
    - Defects and Failures
    - Approach and Responsibilities

  - **Component Testing** (Unit Testing)

    - Focuses on testing components in isolation
    - Requires Test Harnesses and Unit Test Frameworks
    - Normally performed by Developers in their Development Environment

  - **Component Integration Testing** (Unit Integration Testing)

    - Focuses on testing interfaces and interactions between components
    - Heavily dependent on integration strategy approaches:
      - Bottom-Up
      - Top-Down
      - Big-Bang

  - **System Testing**

    - Focuses on overall behavior and capabilities of an entire system or product
      - Functional Testing of End-to-End tasks
      - Non-Functional Testing of quality characteristics
        - Preferable to test on a complete system in a representative test environment (Usability)
    - Simulation of Sub-Systems
    - May be performed by Independent Test Team
    - Related to specifications for the system

  - **System Integration Testing**
    - Focuses on testing Interfaces of the system under test and other systems and external services
    - Requires suitable test environments preferably similar to the Operational Environment
  - **Acceptance Testing**
    - Focuses on validation and on demonstrating readiness for deployment
      - System fulfills the user's business needs
    - Performed by intended users
    - Types of Acceptance Testing:
      - User Acceptance Testing (UAT)
      - Operational Acceptance Testing
      - Contractual and Regulatory Acceptance Testing
      - Alpha Testing
      - Beta Testing

  <a id=222></a>

  ## (2.2.2) Test Types

  - The following tests can be applied to all test levels
  - Different Test Techniques can be used to derive test conditions and test cases for the following tests

  - **Functional Testing**

    - Evaluates performance of component or system function
    - Functions are "what" the test object should do
    - Main Objective:
      - Functional Completeness
      - Functional Correctness
      - Functional Appropriateness

  - **Non-Functional Testing**
    - Evaluates attributes other than functional characteristics of a component or system
    - Tests "How well the system behaves"
    - Appropriate to start early in SDLC
    - Tests are sometimes derived from functional tests
    - Late detection could cause serious threat to success of the project
    - Needs very specific test environment such as Usability Lab for Usability Testing
    - Main Objective:
      - Checking non-functional software quality characteristics
    - Classification of non-functional Software Quality Characteristics:
      - Performance Efficiency
      - Compatibility
      - Usability
      - Reliability
      - Security
      - Maintainability
      - Portability
  - [**Black-Box Testing**](/Chapters/Chapter%204/Section_2.md)
    - Specification-based and derived from documentation external to test object
    - Main Objective:
      - Checking system's behavior against its specification

  -[**White-Box Testing**](/Chapters/Chapter%204/Section_3.md)

  - Structured-based and derived from system's implementation or internal structure (Code, Architecture, Work-Flows, Data flows)
  - Main Objective:
    - Cover underlying structure by the tests to the acceptable level

  <a id=223></a>

  ## Confirmation Testing and Regression Testing

  - **Confirmation Testing**

    - Confirms original defect/bug is fixed
    - Dependent on Risk, testing can be done:
      - Executing all test cases that previously failed due to defect
      - Adding new tests to cover any changes that were needed to fix defect
    - When Time/Money is short, confirmation testing might be restricted to:
      - Exercising steps that reproduce the failure cause by the defect
      - Checking that the failure does not occur

  - **Regression Testing**
    - Confirms no additional defects/bugs are present by changes
    - You should perform an Impact Analysis to optimize the extent of the testing
      - Impact Analysis shows which parts of the software could be affected
    - Regression Test Suites can run many times
    - Number of Regression Test Cases will increase with each iteration or release
    - Great candidate for Automation and should be done early

---

<table width="100%">
<tr>
    <td align="left">
        <a href="#previous-section" style="padding-right: 100px;">Previous</a>
    </td>
    <td align = "center></td>
    <td align="right">
        <a href="#next-section" style="padding-left: 100px;">Next</a>
    </td>
</tr>
</table>

---