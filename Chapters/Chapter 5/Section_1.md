<details>
  <summary>Table of Contents</summary>
  <ul>
    <li><a href="/README.md">Home</a></li>
    <li><a href="Chapter_5_Home.md">Chapter Home</a></li>
    <li><a href="Section_1.md">Section 1</a></li>
    <li><a href="Section_2.md">Section 2</a></li>
    <li><a href="Section_3.md">Section 3</a></li>
    <li><a href="Section_4.md">Section 4</a></li>
    <li><a href="Section_5.md">Section 5</a></li>
  </ul>
</details>

## Section Guide
- [(K2) Exemplify the purpose and content of a test plan](#511)
- [(K1) Recognize how a tester adds value to iteration and release planning](#512)
- [(K2) Compare and contrast entry criteria and exit criteria](#513)
- [(K3) Use estimation techniques to calculate the required test effort](#514)
- [(K3) Apply test case prioritization](#515)
- [(K1) Recall the concepts of the test pyramid](#516)
- [(K2) Summarize the testing quadrants and their relationships with test levels and test types](#517)

<a id=51></a>

## Test Planning

- Test Planning

    <a id=511></a>
    
    ## (5.1.1) Purpose and Content of a Test Plan
    - Test plan describes ____ for a test project:
        - Objectives
        - Resources
        - Processes

    - **Test Plan**:
        - Documents the means and schedule for achieving test objectives
        - Helps to ensure that the performed test activities will meet the established criteria
        - Serves as a means of communication with team members and other stakeholders
        - Demonstrates that testing will adhere to the existing test policy and test strategy 
            - Explains why the testing will deviate from them
    
    - **Test Planning** 
        - Guides the testers' thinking
        - Forces testers to confront future challenges related to:
            - Risks
            - Schedules
            - People
            - Tools
            - Costs
            - Effort
        - Test Plan preparation is useful way to think through the efforts needed to achieve the test project objectives

        - Typical Contents:
            - Context of Testing
                - Scope
                - Test Objectives
                - Constraints
                - Test Basis

            - Assumptions and Constraints of the test project

            - Stakeholders
                - Roles
                - Responsibilities
                - Relevance to testing
                - Hiring and training needs

            - Communication
                - Forms and frequency of communication
                - Documentation templates
            
            - Risk Register
                - Product Risks
                - Project Risks
            
            - Test Approach
                - Test \_\_\_\_:
                    - Levels
                    - Types
                    - Techniques
                    - Deliverables
                    - Data Requirements
                    - Environment Requirements
                - Entry/Exit Criteria
                - Independence of Testing
                - Metrics to be collected
                - Deviations from the organizational test policy and test strategy
            
            - Budget
            - Schedule

    <a id=512></a>

    ## (5.1.2) Tester's Contribution to Iteration and Release Planning
    - In Iterative SDLC's, there are two types of planning:
        - Release Planning
        - Iteration Planning
    
    - **Release Planning**
        - Looks ahead to the release of a products
        - Defines and re-defines the product backlog
        - Refines larger user stories into a set of smaller user stories
        - Serves as the basis for the test approach and test plan across all iterations
        - Testers involved participate in:
            - Writing testable User Stories and [Acceptance Criteria](/Chapters/Chapter%204/Section_5.md)
            - Project and Quality [Risk Analyses](Section_2.md)
            - [Estimate](#514) test effort associated with User Stories
            - Determine Test Approach
            - Plan the testing for the release
    
    - **Iteration Planning**
        - Looks ahead to the end of a single iteration
        - Concerned with the iteration backlog
        - Testers involved participate in:
            - Detailed risk analysis of User Stories
            - Determine the testability of User Stories
            - Break down User Stories into tasks (particularly testing tasks)
            - Estimate test effort for all testing tasks
            - Identify and Refine functional and non-functional aspects of the test object

    <a id=513></a>

    ## (5.1.3) Entry Criteria and Exit Criteria
    - Both Entry and Exit Criteria should be defined for each test level
    - Both will differ based on the test objectives

    - **Entry Criteria**
        - Defines the preconditions for undertaking a given activity
        - If it is not met, it is likely that the activity will prove to be more:
            - Difficult
            - Time-Consuming
            - Costly
            - Risky
        - Typical Entry Criteria:
            - Availability of Resources
                - People
                - Tools
                - Environments
                - Test Data
                - Budget
                - Time
            - Availability of Software
                - Test Basis
                - Testable Requirements
                - User Stories
                - Test Cases
            - Initial Quality Level of a Test Object
                - All Smoke Tests have passed
        
    - **Exit Criteria**
        - Defines what must be achieved in order to declare an activity completed
        - Typical Exit Criteria:
            - Measures of Thoroughness
                - Achieved level of Coverage
                - Number of Unresolved Defects
                - Defect Density
                - Number of Failed Test Cases
            - Completion Criteria
                - Planned Tests have been executed
                - Static Testing has be performed
                - All defects found are reported
                - All Regression Tests are automated
            - Running out of time or budget
        - If stakeholders have reviewed and accepted the risks to go live, all Exit Criteria do not need to be satisfied

    - **Agile Software Development**
        - Exit Criteria is known as **Definition of Done**
            - Defines the team's objective metrics for a releasable item
        - Entry Criteria is known as **Definition of Ready**
            - Criteria that must be fulfilled to start the development and/or testing activities

    <a id=514></a>
    
    ## Estimation Techniques
    - Predicting the amount of test-related work needed to meet the objectives of a test project
    - Important to make it clear to stakeholders that the estimate is based on a  number of assumptions and is always subject ot estimation error
    - Estimation for small tasks are usually more accurate than for large tasks
    - When estimating for large tasks, it can be decomposed into a set of smaller tasks, then estimated

        ## Estimation based on Ratios
        - Metrics-Based Technique
        - Figures are collected from previous projects within the organization
            - Allows teams to derive "standard" ratios for similar projects
        - Ratios of an organization's own projects (taken from historical data) are generally the best source to use for estimation process
            - These ratios can be used to estimate the test effort for the new project
            - Example:
                - Previous Project - Development-to-Test Effort ratio was 3:2
                - Current Project - Development Effort is expected to be 600 person-days
                - Test Estimate - 400 person-days
                    - 600 / 3 = 200
                    - 200 * 2 = 400

        ## Extrapolation
        - Metrics-Based Technique
        - Measurements are made as early as possible in the current project to gather data
        - Effort required for the remaining work can be approximated by extrapolating this date with enough observations
            - Usually by applying a mathematical model
        - Very suitable in Iterative SDLCs
        - Example:
            - Team may extrapolate the test effort in the forthcoming iteration as the averaged effort from the last three iterations
        
        ## Wideband Delphi
        - Iterative, Expert-Based Technique
        - Experts make Experience-Based Estimations
        - Each expert in isolation, estimates effort
        - Results are collected and if there are deviations that are out of range of the agreed upon boundaries, experts will discuss their estimates
        - Each expert is then asked to re-estimate, in isolation, based on the feedback
        - Repeated until consensus is made

        - **Planning Poker**
            - A variant of Wideband Delphi
            - Commonly used in Agile Software Development
            - Estimates are usually made using cards with numbers that represent the effort size

        ## Three-Point Estimation
        - Expert-Based Technique
        - Three estimations are made by experts:
            - Most Optimistic (A)
            - Most Likely (M)
            - Most Pessimistic (B)
        - Final Estimate (E) = (A + 4*M + B) / 6
        - An advantage of this technique is that it allows the experts to calculate the measurement error
            - SD = (B - A) / 6
        
        - Example: 
            - A = 6
            - M = 9
            - B = 18
            - Estimation: 
                - E = (6 + (4 * 9) + 18) / 6
                - E = 10
            - Measurement Error:
                - SD = (18 - 6) / 6
                - SD = 2
            - Final Answer:
                - 10 +- 2
        
    <aa id=515></a>

    ## (5.1.5) Test Case Prioritization
    - Test Cases and Test procedures are specified and assembled into Test Suites
        - Test Suites are then arranged in a Test Execution Schedule
            - Defined by the order they are to be run
    - Different factors are taken into account
    - Most commonly used Test Case Prioritization Strategies:
        - Risk-Based Prioritization
            - Order of Test Execution is based on results of [Risk Analysis](Section_2.md#523)
            - Test Cases covering the most important risks are executed first

        - Coverage-Based Prioritization
            - Order of Test Execution is based on Coverage (Statement Coverage)
            - Test Cases achieving the highest coverage are executed first
            - Additional Coverage Prioritization
                - Another variant of Coverage-Based Prioritization
                - Test Case achieving the highest coverage is executed first
                - Each subsequent test case is the one that achieves the highest additional coverage

        - Requirements-Based Prioritization
            - Order of Test Execution is based on the priorities of the requirements traced back to the corresponding test cases
            - Requirement priorities are defined by stakeholders
            - Test cases related to the most important requirements are executed first
        
    - Ideally Test Cases would be ordered to run based on their priority levels using one of the above-mentioned prioritization strategies
        - If test cases or features being tested have dependencies, this may not work
    - If a test case with a higher priority is dependent on a test case with a lower priority, the lower priority test case must be executed first
    - Order of Test execution must also take into account of the availability of resources
        - Required Test Tools
        - Required Test Environments
        - Required People that may only be available for a specific time window

    <a id=516></a>
    
    ## (5.1.6) Test Pyramid
    - Model that shows different tests may have different granularity (level of detail)
    - Supports team in test automation and in test effort allocation by showing that different goals are supported by different levels of test automation
    - Pyramid layers represent groups of tests
        - The higher the layer, the lower:
            - Test Granularity
            - Test Isolation
            - Test Execution Time
        - Bottom Layer Tests:
            - Small
            - Isolated
            - Fast
            - Check a small piece of functionality
            - A lot are needed to achieve a reasonable coverage
        - Top Layer Tests:
            - Complex
            - High-level
            - End-to-End Tests
            - Generally slower than lower layer tests
            - Checks a large piece of functionality
            - Fewer are needed to achieve reasonable coverage
        - Number and Naming of layers may differ:
            - Original Test Pyramid Model defined three layers:
                - Unit Tests
                - Services Tests
                - UI Tests
            - Another popular model defines the three layers:
                - Unit (Component) Tests
                - Integration (Component Integration) Tests
                - End-to-End Tests
            - [Other Test Levels](/Chapters/Chapter%202/Section_2.md#221) can be used
    
    <a id=517></a>

    ## (5.1.7) Testing Quadrants
    - With Agile, Testing Quadrants are grouped by the test levels with the appropriate:
        - Test Types
        - Activities
        - Test Techniques
        - Work Products
    - Model supports test management in visualizing this
        - Ensures that all appropriate test types and test levels are included in the SDLC
        - Understands that some test types are more relevant to certain test levels than other
        - Provides a way to differentiate and describe the types of test to:
            - All Stakeholders
            - Developers
            - Testers
            - Business Representatives
    - Tests can be Business Facing or Technology Facing
    - Tests support the team (Guide the development) or critique the product (Measure its behavior against the expectations)
        - These two viewpoints determines the four quadrants:
            - **Quadrant Q1** (Technology Facing, support the team)
                - Contains:
                    - Component
                    - Component Integration Tests
                - Tests should be automated and included in CI process

            - **Quadrant Q2** (Business Facing, support the team)
                - Contains: 
                    - Functional tests
                    - Examples
                    - User Story Tests
                    - User Experience Prototypes
                    - API Testing
                    - Simulation
                - These tests check the acceptance criteria
                - Tests can be manual or automated

            - **Quadrant Q3** (Business Facing, critique the product)
                - Contains:
                    - Exploratory Testing
                    - Usability Testing
                    - User Acceptance Testing
                - User Oriented and often manual

            - **Quadrant Q4** (Technology Facing, critique the product)
                - Contains:
                    - Smoke Tests
                    - Non-Functional Tests (except Usability Tests)
                - Test are often automated