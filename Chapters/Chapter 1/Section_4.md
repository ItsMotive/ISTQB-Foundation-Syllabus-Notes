<details>
  <summary>Table of Contents</summary>
  <ul>
    <li><a href="/README.md">Home</a></li>
    <li><a href="Chapter_1_Home.md">Chapter Home</a></li>
    <li><a href="Section_1.md">Section 1</a></li>
    <li><a href="Section_2.md">Section 2</a></li>
    <li><a href="Section_3.md">Section 3</a></li>
    <li><a href="Section_4.md">Section 4</a></li>
    <li><a href="Section_5.md">Section 5</a></li>
  </ul>
</details>

## Section Guide

- [(K2) (1.4.1) Summarize the Different Test Activities and Tasks](#141)
- [(K2) (1.4.2) Explain the Impact of Context on the Test Process](#142)
- [(K2) (1.4.3) Differentiate the Testware that Supports the Test Activities](#143)
- [(K2) (1.4.4) Explain the Value of Maintaining Traceability](#144)
- [(K2) (1.4.5) Compare the Different Roles in Testing](#145)

<a id="14"></a>

## (1.4) Test Activities, Testware, and Test Roles

- Without a common set of **test activities**, testing can become less likely to reach **test objectives**.
- A set of **test activities** create a **test process**.
- **Test Planning:**
  - Test process can be tailored to a given situation based on various factors:
    - Which test activities are included in the test process
    - How test activities are implemented
    - When test activities occur
- [ISO/IEC/IEEE 29119-2 2021 Standard](https://ieeexplore.ieee.org/document/9687474) provides more info about test processes.

  <a id="141"></a>

  ## (1.4.1) Test Activities and Tasks

  - Although many of the to be listed test activities seem to follow a logical sequence, they are often implemented iteratively or in parallel.
  - The testing activities need to be tailored to the system or the project.
  - **Test Process** consists of these main groups of activities:

    ### Test planning

    - Defining test objectives
    - Selecting the best approach to achieve the objective within the constraints defined

    ### Test Monitoring and Control

    - **Test Monitoring:**
      - Continuously checking all test activities
      - Comparing actual progress against test plan
    - **Test Control:**
      - Taking necessary actions to meet test objective

    ### Test Analysis

    - Analyze the test basis to identify testable features.
    - Define and Prioritize associated test conditions, together with related risks and risk levels.
    - Test Basis and Test Objects are evaluated to identify defects and assess testability.
    - Answers the question, "What to test" in terms of measurable coverage criteria.

    ### Test Design

    - Turning **Test Conditions** into **Test Cases** and other **Testware**.
    - Identifying coverage items as a guide to specify test case inputs.
    - Defining test data requirements.
    - Designing test environment.
    - Identifying other required infrastructure and tools.
    - [Testing Techniques](Chapter%204.md) can support test designing.
    - Answers the question, "How to test?"

    ### Test Implementation

    - Creating/Gathering testware for Test Execution.
      - EX: Test Data
    - Organized into Test Procedures.
      - Prioritized and Arranged within Test Execution Schedule for more efficient Test Execution.
    - Assembled into Test Suites
    - Manual and Automated Test Scripts are created here.

    ### Test Execution

    - Running tests according to Test Execution Schedule (Test Runs).
    - Comparing actual test results with expected.
    - Logging test results and defects.
    - Manual or Automated Testing
    - Continuous or Pair Testing Sessions

    ### Test Completion

    - Usually occurs at **Project Milestones** for:
      - Unresolved Defects
      - Change Requests
      - Product Backlog items created
      - Project Milestone Examples:
        - Release
        - End of Iterations
        - Test Level Completion
    - Identifying, Archiving, or Handing over Testware for future use.
    - Test Environment is shutdown and archived in an agreed state.
    - Review Test Activities for lessons learned and improvements for future iterations, releases, or projects.
    - Test Completion Report is created and shared with stakeholders.

  <a id="142"></a>

  ## (1.4.2) Test Process in Context

  - Testing is funded by stakeholders and the final goal is to fulfill the stakeholders' business requirements.
  - Testing will depend on:
    - Stakeholders (needs, expectations, requirements, willingness to cooperate, etc.)
    - Team members (skills, knowledge, level of experience, availability, training needs, etc.)
    - Business domain (criticality of the test object, identified risks, market needs, specific legal regulations, etc.)
    - Technical factors (type of software, product architecture, technology used, etc.)
    - Project constraints (scope, time, budget resources, etc.)
    - Organizational factors (organization structure, existing policies, practices used, etc.)
    - Software Development Lifecycle (engineering practices, development methods, etc.)
    - Tools (availability, usability, compliance, etc.)
  - These factors impact test-related issues, such as:
    - Test Strategy
    - Test Techniques used
    - Degree of Test Automation
    - Required level of coverage
    - Level of Test Documentation detail
    - Reporting
    - etc.

  <a id="143"></a>

  ## (1.4.3) Testware

  - Created as output **Work Products** from [Test Activities](#141).
  - No company creates and manage their Work Products the same.
  - Proper management of configuration ensures consistency and integrity of Work Products.
  - Some Work Products include:

    - **Test planning Work Products**

      - Test Plan
      - Test Schedule
      - Risk Register
        - List of risks with:
          - Risk Likelihood
          - Risk Impact
          - [Risk Mitigation](Chapter%205#2) Info
      - [Entry/Exit Criteria](Chapter%205#1)

    - **Test Monitoring and Control Work Products**

      - [Test Progress Reports](Chapter%205#Section3.2)
      - [Documentation of Control Directives](Chapter%205#3)
      - [Risk Information](Chapter%205#2)

    - **Test Analysis Work Products**

      - (Prioritized) Test Conditions
        - Acceptance Criteria
      - Defect Reports with Test Basis defects (if not fixed directly)

    - **Test Design Work Products**

      - (Prioritized) Test Cases
      - Test Charters
      - Coverage Items
      - Test Data Requirements
      - Test Environment Requirements

    - **Test Implementation Work Products**

      - Test Procedures
      - Automated Test Scripts
      - Test Suites
      - Test Data
      - Test Execution Schedule
      - Test Environment Variables
        - Stubs
        - Drivers
        - Simulators
        - Service Virtualizations

    - **Test Execution Work Products**

      - Test Logs
      - [Defect Reports](Chapter%205#5)

    - **Test Completion Work Products**
      - [Test Completion Report](Chapter%205#532)
      - Action Items for Improvement
      - Documented Lessons Learn
      - Change Requests
        - EX: Product Backlog Items

  <a id="144"></a>

  ## (1.4.4) Traceability between the Test Basis and Testware

  - Important to establish and maintain traceability throughout the test process.
    - Test Basis Elements
    - Testware associated with:
      - Test Conditions
      - Risks
      - Test Cases
      - etc.
  - Accurate traceability supports coverage evaluation.
  - Measurable Coverage Criteria should be defined in Test Basis.
    - Traceability of Test Cases to Requirements verify Requirements are covered by Test Cases.
    - Traceability of Test Results to Risks evaluate level of Residual Risk in Test Objects.
  - Traceability in general provides:
    - Information to assess Product Quality
    - Process Capability
    - Project Progress against business goals
  - Good Traceability allows for:
    - Determining impact of changes
    - Facilitates Test Audits
    - Meet IT Governance Criteria
    - Test Progress and Test Completion Reports more easily understandable
      - Includes Status of Test Basis Elements
    - Assist in communicating Technical Aspects of Testing to Stakeholders

  <a id="145"></a>

  ## (1.4.5) Roles in Testing

  - There are two (2) Principle Roles: **Test Management** and **Testing**
  - Different people may take on these roles at different times.
    - Test Management Role can be performed by:
      - Team Leader
      - Test Manager
      - Development Manager
      - etc.
  - One (1) person can also take on both roles at the same time.

  - **Test Management Role:**

    - Overall responsible for:
      - Test Process
      - Test Team
      - Leadership of Test Activities
    - Mainly focused on:
      - Activities of Test Plan
      - Test Monitoring
      - Test Controlling
      - Test Completion
    - Agile Example:
      - Test Management tasks may be handled by Agile Team
      - Tasks for multiple teams or entire organization may be performed by Test Managers outside of Development Team

  - **Testing Role**
    - Overall responsible for:
      - Engineering (Technical) aspect of Testing
    - Mainly focused on Activities of:
      - Test Analysis
      - Test Design
      - Test Implementation
      - Test Execution
