# Chapter 1: Fundamentals of Testing

## Description 
- It is estimated that you should take around 180 minutes (3 Hours) to learn.
- In this chapter learn and understand:
    - The basic principles related to testing
    - The reasons why testing is required
    - What the test objectives are
    - Test Process
    - Major Test Activities
    - Testware
    - Essential Skills for Testing
- Knowledge Levels
    - K1: Remember - You should remember/recognize a term or a concept
    - K2: Understand - You should be able to select an explanation for a statement related to the question topic

## Learning Objectives for Chapter 1
- [What is Testing?](#11)
    - [(K1) Identify Typical Test Objectives](#111)
    - [(K2) Differentiate Testing from Debugging](#112)
- [Why is Testing Necessary?](#12)
    - [(K2) Exemplify Why Testing is Necessary](#121)
    - [(K1) Recall the Relation between Testing and Quality Assurance](#122)
    - [(K2) Distinguish between Root Cause, Error, Defect, and Failure](#123)
- [Testing Principles](#13)
    - [(K2) Explain the Seven Testing Principles](#131)
- [Test Activities, Testware, and Test Roles](#14)
    - [(K2) Summarize the Different Test Activities and Tasks](#141)
    - [(K2) Explain the Impact of Context on the Test Process](#142)
    - [(K2) Differentiate the Testware that Supports the Test Activities](#143)
    - [(K2) Explain the Value of Maintaining Traceability](#144)
    - [(K2) Compare the Different Roles in Testing](#145)
- [Essential Skills and Good Practices in Testing](#15)
    - [(K2) Give Examples of the Generic Skills Required for Testing](#151)
    - [(K1) Recall the Advantages of the Whole Team Approach](#152)
    - [(K2) Distinguish the Benefits and Drawbacks of Independence of Testing](#153)

<a id="11"></a>
## (1.1) What is Testing? 

**Software Testing...**
- Assesses Software Quality and helps reducing the risk of software failure.
- Set of activities to find defects and evaluate the quality of software artifacts.
- May be [Static](Chapter%203.md) or [Dynamic](Chapter%204.md).
- Is technical and needs to be properly [Planned, Managed, Estimated, Monitored, and Controlled](Chapter%205.md).
- Is an intellectual activity, requiring testers to have specialized knowledge, use analytical skills, and apply critical thinking and systems thinking. 
- Uses [Tools](Chapter%206.md)

    <a id="111"></a>
    ## (1.1.1) Test Objectives
    - **Typical Objectives:**
        - Evaluating work products such as requirements, user stories, designs, and code.
        - Triggering failures and finding defects.
        - Ensuring required coverage of a test object.
        - Reducing the level of risk of inadequate software quality.
        - Verifying whether specified requirements have been fulfilled.
        - Verifying that a test object complies with contractual, legal, and regulatory requirements.
        - Providing information to stakeholders to allow them to make informed decisions.
        - Building confidence in the quality of the test object.
        - Validating whether the test object is complete and works as expected by the stakeholders.

    - **Objectives are dependent on context:**
        - Work product being tested
        - Test Level
        - Risks
        - SDLC being followed
        - Factors related to the business context:
            - Corporate Structure
            - Competitive Considerations
            - Time to Market
    
    <a id="112"></a>
    ## (1.1.2) Testing and Debugging
    - **Testing:** Triggers failure that are caused by defects in the software or finds defects in the test object.

    - **Debugging:** Finds causes for defect/failure, analyzes, and eliminates them.

    - **Debugging Process:**
        - Reproduction of a failure
        - Diagnosis (Finding Root Cause)
        - Fixing the cause

    - **Subsequent Confirmation Testing** - Initial Tester checks whether the fixes resolved the problem.
    - **Subsequent Regression Testing** - Checks whether the fixes are causing failures in other parts of the test object. [(Section 2.2.3)](Chapter%202.md#223)
    - With Static Testing, there is no need for reproduction or diagnosis, since it directly finds defects and cannot cause failures. 

<a id="12"></a>

## (1.2) Why is Testing necessary?
- Testing components, systems, and associated documentation helps to identify defects in software.
- Testing's contribution to success should not be restricted to the test team's activities.

- **Testing:**
    - Helps achieve agreed upon goals within:
        - Set Scope
        - Time
        - Quality
        - Budget Constraint

    <a id="121"></a>
    ## (1.2.1) Testing's Contributions to Success
    - Testing indirectly contributes to high quality test objects.
    - Test objects contribute to decisions to move to next stages of SDLC, such as release decision.

    - **Testing Provides:**
        - Cost-Effective means of detecting defects
        - Means of directly evaluating the quality of a test object at various stages in the SDLC
        - Users with indirect representation on the development project
        - Means of meeting contractual or legal requirements
        - Means of complying with regulatory standards

    <a id="122"></a>
    ## (1.2.2) Testing and Quality Assurance (QA)
    - Testing and Quality Assurance are **not the same**.
    - Test results are used by QA and QC.

    - **Quality Control (QC)**
        - **Product-Oriented**
        - **Corrective Approach** that focuses on activities to achieve appropriate levels of quality
        - **Test results** are used to fix defects
        - Forms of QC:
            - Testing
            - Model Checking
            - Proof of Correctness
            - Simulation
            - Prototyping
    
    - **Quality Assurance (QA)**
        - **Process-Oriented**
        - **Preventive Approach** that focuses on implementation and improvement of processes
        - **Test results** are used to provide feedback on development and test processes
        - If a good process is followed correctly, then a good product will be made
        - Applies to development and testing processes
        - Responsibility of everyone on the project

    <a id="123"></a>
    ## (1.2.3) Errors, Defects, Failures, and Root Causes
    - **Errors (Mistakes)** produce **Defects (Faults, Bugs)** which results in **Failures**.

    - **Errors** 
        - Occur due to:
            - Time Pressure
            - Complexity of work products
            - Processes
            - Infrastructure
            - Interactions
            - Tired or lack of adequate training

    - **Defects**
        - Undetected defects produced in early stages of SDLC, often lead to defects later.
        - Can cause failures:
            - Always
            - Under specific circumstances
            - Never
        - Can be found in documentation:
            - Requirements specification
            - Test Script
            - Source Code
            - Build Files

    - **Failures**
        - **Errors** and **Defects** are not the only cause.
            - EX: Firmware defects
    
    - **Root Cause**
        - Fundamental reason for a problem or problems.
        - Identified through **Root Cause Analysis**.

<a id="13"></a>

## (1.3) Testing Principles
### 1. Testing shows the presence, not the absence of defects.
- Testing can:
    - Show defects are present
    - Reduce probability of defects remaining undiscovered
- Testing cannot prove:
    - There are no defects
    - Test object correctness
    
### 2. Exhaustive testing is impossible.
- Testing everything is not feasible except in trivial cases.
- Instead use ____ to focus test efforts:
    - [Test Techniques](Chapter%204.md)
    - [Test Case Prioritization](Chapter%205#515)
    - [Risk-Based Testing](Chapter%205#52)

### 3. Early testing saves time and money
- Defects found early in the SDLC will reduce defects later on whether related or not.
- Both Static and Dynamic Testing should be done as soon as possible.

### 4. Defects cluster together.
- Most defects discovered or defects responsible for failures are usually in a small number of system components.
    - Phenomenon is called Pareto Principle.
- For **Risk-Based Testing**, **Predicted** and **Actual** defect clusters observed during testing are an important.

### 5. Tests wear out.
- Repeating the same tests over and over make them less effective when trying to find new defects.
- To work around this:
    - Modify existing tests
    - Modify existing test data
    - Create new tests
- Repeating tests such as Automated Regression **can** be beneficial

### 6. Testing is context dependent.
- No universally correct approach to testing.

### 7. Absence-of-Defects Fallacy.
- It is a misconception that software verification will result in the success of a system.
- Even testing all specified requirements and fixing all defects found, it does not guarantee:
    - System fulfills users' needs and expectations
    - Achieve customer's business goals
- Verification and Validation should both be done.

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
    - Created as output **Work Products** from [Test Activities](#test-activities-and-tasks).
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
                    - [Risk Mitigation](Chapter%205#Section2) Info
            - [Entry/Exit Criteria](Chapter%205#Section1)

        - **Test Monitoring and Control Work Products**
            - [Test Progress Reports](Chapter%205#Section3.2)
            - [Documentation of Control Directives](Chapter%205#Section3)
            - [Risk Information](Chapter%205#Section2)

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
            - [Defect Reports](Chapter%205#Section5)

        - **Test Completion Work Products**
            - [Test Completion Report](Chapter%205#Section3.2)
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

<a id="15"></a>

## (1.5) Essential Skills and Good Practices in Testing
- Good Testers should:
    - Have essential skills to do the job
    - Effective team players
    - Perform testing on different levels of Test Independence

    <a id="151"></a>
    ## (1.5.1) Generic Skills Required for Testing
    - Testers will often be the bearer of bad news. Therefore communication is a crucial skill. 

    - **Testing Knowledge**
        - Increases effectiveness of testing by using Test Techniques

    - **Thoroughness, Carefulness, Curiosity, Attention to Detail, being Methodical**
        - Helps to identify defects, especially hard to find ones. 

    - **Good Communication Skills, Active Listening, Being a Team Player**
        - Helps to interact effectively with Stakeholders
        - Helps to convey information to others
        - Helps to report and discuss defects

    - **Analytical Thinking, Critical Thinking, Creativity**
        - Increases effectiveness of testing
    
    - **Technical Knowledge**
        - Increases effectiveness of testing by using appropriate Test Tools

    - **Domain Knowledge**
        - Helps to understand and communicate with end users/business representatives

    <a id="152"></a>
    ## (1.5.2) Whole Team Approach
    - Dependent on Context, Whole Team Approach is not always appropriate.
        - EX: Safety Critical, a high level of test independence may be needed.
    - Any team member with the necessary knowledge or skills can perform any task.
    - Whole team is responsible for Quality.
    - Benefits:
        - Improves team dynamics
        - Enhances communication and collaboration
        - Creates synergy 
    
    <a id="153"></a>
    ## (1.5.3) Independence of Testing
    - Usually best to carry out testing with multiple levels of Independence
        - Developers performing Component and Component Integration Testing
        - Test Team performing System and System Integration Testing
        - Business Representatives performing Acceptance Testing

    - Work Products Tested by:
        - Original Author (**No Independence**)
        - Author's peers from the same team (**Some Independence**)
        - Testers outside of Author's team, but within organization (**High Independence**)
        - Testers outside of the organization (**Very High Independence**)

    - Drawbacks of Independent Testers:
        - Lack of collaboration
        - Communication Problems
        - Adversarial relationship with Development Team
        - Developers losing sense of Responsibility of Quality
        - Testers being considered as bottlenecks
        - Testers being blamed for delays in release
    - Benefits of Independent Testers:
        - Testers are more likely to find different kinds of failures/defects 
            - Due to different backgrounds, technical perspectives, and biases
        - Testers can verify, challenge, or disprove assumptions