<details>
  <summary>Table of Contents</summary>
  <ul>
    <li><a href="/README.md">Home</a></li>
    <li><a href="Chapter_2_Home.md">Chapter Home</a></li>
    <li><a href="Section_1.md">Section 1</a></li>
    <li><a href="Section_2.md">Section 2</a></li>
    <li><a href="Section_3.md">Section 3</a></li>
  </ul>
</details>

## Section Guide

- [(K2) (2.1.1) Explain the impact of the chosen SDLC on testing](#211)
- [(K1) (2.1.2) Recall good testing practices that apply to all SDLC](#212)
- [(K1) (2.1.3) Recall the examples of Test-First approaches to development](#213)
- [(K2) (2.1.4) Summarize how DevOps might have an impact on testing](#214)
- [(K2) (2.1.5) Explain the Shift-Left Approach](#215)
- [(K2) (2.1.6) Explain how retrospectives can be used as a mechanism for process improvement](#216)

<a id="21"></a>

## (2.1) Testing in the Context of SDLC

- **SDLC Models:**
  - Sequential Development Models
    - Waterfall Model
    - V-Model
  - Iterative Development Models
    - Spiral Model
    - Prototyping
    - Agile
  - Incremental Development Models
    - Unified Process
- Software Development Methods and Agile Practices:

  - Acceptance Test-Driven Development (ATDD)
  - Behavior-Driven Development (BDD)
  - Domain-Driven Development (DDD)
  - Extreme Programming (XP)
  - Feature-Driven Development (FDD)
  - Test-Driven Development (TDD)
  - Kanban
  - Lean IT
  - Scrum

  <a id="211"></a>

  ## (2.1.1) Impact of the SDLC on Testing

  - SDLC choice impacts:

    - Scope and Timing of Test Activities
      - Test Levels
      - Test Types
    - Level of detail of Test Documentation
    - Choice of Test Techniques and Test Approach
    - Extent of Test Automation
    - Role and Responsibilities of a Tester

  - With **Sequential Development Models**:

    - Initial Phase Testers participate in:
      - Requirement Reviews
      - Test Analysis
      - Test Design
    - Later Phases:
      - Executable Code is created
    - Dynamic Testing usually cannot be performed early in SDLC

  - With **Iterative** and **Incremental Development Models**:
    - During each iteration:
      - Deliver a working prototype or product increment
      - Static and Dynamic Testing are performed at all test levels
      - Frequent delivery of increments require fast feedback and extensive Regression Testing

  - Within **Agile**:
    - Changes may occur throughout the project
    - Regression Tests are made easier through:
      - Lightweight Work Product Documentation
      - Extensive Test Automation 
    - Most Manual Testing is done with [Experience-Based Test Techniques](/Chapters/Chapter%204/Section_4.md#44)
      - Extensive prior Test Analysis and Design is not required

  <a id="212"></a>

  ## SDLC and Good Testing Practices
  - Good practices independent of chosen SDLC:
    - For every Software Development Activity, there should be a corresponding Test Activity to ensure all development activities are subject to Quality Control
    - Different [Test Levels](/Chapters/Chapter%202/Section_2.md#221) have specific and different Test Objectives to allow testing to be appropriately comprehensive while avoiding redundancy
    - Test Analysis and Design for a given test level beings during the corresponding development cycle of the SDLC, so testing can adhere to the principle of [Early Testing](/Chapters/Chapter%201/Section_3.md#13)
    - Testers are involved in reviewing Work Products as soon as drafts of this documentation are available, so that this earlier testing and defect detection can support the [Shift-Left Strategy](#215)

  <a id="213"></a>

  ## Testing as a Driver for Software Development
  - **TDD**, **ATDD**, and **BDD**:
    - Similar Development Approaches
    - Tests are defined as a means of directing development
    - Implements of [Early Testing](/Chapters/Chapter%201/Section_3.md)
    - Follows [Shift-Left Approach](#215)
    - Support Iterative Development Model
    - Tests may become automated tests to ensure code quality for any future changes

  - **Test-Driven-Development (TDD)**
    - Directs coding through Test Cases
    1. Tests are written first
    2. Then code is written to satisfy tests
    3. Then tests and codes are refactored

  - [**Acceptance Test-Driven Development (ATDD)**](/Chapters/Chapter%204/Section_5.md#453)
    - Tests come from Acceptance Criteria as part of the System Design Process
    - Tests are written before the part of the application is developed to satisfy the tests

  - **Behavior-Driven Development (BDD)**
    - Based on the desired behavior of an application
    - Test Cases are usually written in Given/When/Then Format
    - Test Cases are automatically translated to executable tests

  <a id="214"></a>

  ## DevOps and Testing
  - Even though DevOps comes with a high level of Automated Testing, Manual testing will still be needed.
  - **DevOps**
    - An organizational approach aiming to create synergy by getting development and operations to work together to achieve common goals
    - Promotes team autonomy, fast feedback, integrated tool chains, and technical practices like CI/CD
    - Enables teams to build, test, and release high quality code faster

  - Benefits of DevOps from a Testing Perspective:
    - Fast feedback on code quality and changes affecting existing code
    - CI promotes [Shift-Left Approach](#215) by encouraging developers to submit high quality code accompanied by component tests and static analysis
    - Promotes automated processes like CI/CD that facilitate establishing stable test environments
    - Increases the view on non-functional characteristics
      - Performance
      - Reliability
    - Automation through a delivery pipeline reduces the need for repetitive manual testing
    - Minimized risk in Regression due to the scale and range of Automated Regression Tests

  - DevOps risks and challenges:
    - DevOps delivery pipeline must be defined and established
    - CI/CD Tools must be introduced and maintained
    - Test automation required additional resources and may be difficult to establish and maintain

  <a id=215></a>

  ## Shift Left Approach
  - Sometimes used as a referral of [Early Testing Principle](/Chapters/Chapter%201/Section_3.md)
  - This approach may result in extra training, effort, and/or costs earlier in the process, but is expected to save efforts and/or costs later in the process
  - Suggests that testing should be done earlier in the SDLC
    - Not waiting for code to be implement
    - Not waiting for components to be integrated
  - Does not mean later testing should be neglected
  - Good Practices to achieve Shift-Left in Testing:
    - Reviewing specification from testing perspective
      - Reviews often find potential defects such as ambiguities, incompleteness, and inconsistencies
    - Writing test cases before the code is written
    - Running code in test harness during code implementation
    - Using CI/CD
      - Fast feedback and automated component tests
    - Completing static analysis of source code prior to dynamic testing, or as part of an automated process
    - Performing non-functional testing starting at the component test level, where possible

  <a is=216></a>

  ## Retrospectives and Process Improvement
  - **Retrospective** are end of Project/Iteration reviews.
    - Critical for successful implementation of CI
    - Results should be recorded and are normally part of the [Test Completion Report](/Chapters/Chapter%205/Section_3.md#532)
  
  - Participants:
    - Testers
    - Developers
    - Architects
    - Product Owner
    - Business Analyst
  - Discussion:
    - What was successful and be retained
    - What was not successful and could be improved
    - How to incorporate the improvements and retain the success in the future
  - Benefits for testing:
    - Increased Test Effectiveness/Efficiency (By implementing suggestions for process improvement)
    - Increased quality of testware (By jointly reviewing the test process)
    - Team bonding and learning
    - Improved quality of the test basis
    - Better cooperation between development and testing