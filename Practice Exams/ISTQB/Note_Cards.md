<style>
details summary {
    font-weight: bold;
}
</style>


<!-- #region Section 1.4.1 -->

## Test Activities and Tasks [(1.4.1)](/Chapters/Chapter%201/Section_4.md#141)

<details>
  <summary>Test Planning</summary> 

- Define test objectives.
- Select the best approach to achieve objectives within constraints.

</details>

<details>
  <summary>Test Monitoring and Control</summary>

**Test Monitoring:**
- Continuously check all test activities.
- Compare actual progress against the test plan.

**Test Control:**
- Take actions to meet test objectives.

</details>

<details>
  <summary>Test Analysis</summary>

- Analyze the test basis to identify testable features.
- Define and prioritize test conditions with related risks.
- Evaluate Test Basis and Test Objects to identify defects and assess testability.
- Answer "What to test" with measurable coverage criteria.

</details>

<details>
  <summary>Test Design</summary>

- Turn Test Conditions into Test Cases and other Testware.
- Identify coverage items to specify test case inputs.
- Define test data requirements.
- Design test environment and identify required infrastructure and tools.
- Use [Testing Techniques](Chapters/Chapter%204/Chapter_4_Home.md) for support.
- Answer "How to test?"

</details>

<details>
  <summary>Test Implementation</summary>

- Create/gather testware for test execution (e.g., Test Data).
- Organize into Test Procedures and arrange within the Test Execution Schedule.
- Assemble into Test Suites.
- Create manual and automated test scripts.

</details>

<details>
  <summary>Test Execution</summary>

- Run tests according to the Test Execution Schedule.
- Compare actual test results with expected results.
- Log test results and defects.
- Perform manual or automated testing.
- Conduct continuous or pair testing sessions.

</details>

<details>
  <summary>Test Completion</summary>

- Occurs at Project Milestones:
  - Unresolved Defects
  - Change Requests
  - Product Backlog items
  - Milestones Examples: Release, End of Iterations, Test Level Completion
- Identify, archive, or hand over testware for future use.
- Shut down and archive the test environment.
- Review test activities for lessons learned and improvements.
- Create and share a Test Completion Report with stakeholders.

</details>

<!-- #endregion -->

<!-- #region Section 1.4.3 -->

## Testware [(1.4.3)](/Chapters/Chapter%201/Section_4.md#143)

<details>
  <summary>Testware Overview</summary>

- Created as output **Work Products** from [Test Activities](#141).
- No company creates and manages their Work Products the same.
- Proper management of configuration ensures consistency and integrity of Work Products.

</details>

<details>
  <summary>Test Planning Work Products</summary>

- Test Plan
- Test Schedule
- Risk Register
  - List of risks with:
    - Risk Likelihood
    - Risk Impact
    - [Risk Mitigation](Chapter%205#2) Info
- [Entry/Exit Criteria](Chapter%205#1)

</details>

<details>
  <summary>Test Monitoring and Control Work Products</summary>

- [Test Progress Reports](Chapter%205#Section3.2)
- [Documentation of Control Directives](Chapter%205#3)
- [Risk Information](Chapter%205#2)

</details>

<details>
  <summary>Test Analysis Work Products</summary>

- (Prioritized) Test Conditions
  - Acceptance Criteria
- Defect Reports with Test Basis defects (if not fixed directly)

</details>

<details>
  <summary>Test Design Work Products</summary>

- (Prioritized) Test Cases
- Test Charters
- Coverage Items
- Test Data Requirements
- Test Environment Requirements

</details>

<details>
  <summary>Test Implementation Work Products</summary>

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

</details>

<details>
  <summary>Test Execution Work Products</summary>

- Test Logs
- [Defect Reports](Chapter%205#5)

</details>

<details>
  <summary>Test Completion Work Products</summary>

- [Test Completion Report](Chapter%205#532)
- Action Items for Improvement
- Documented Lessons Learned
- Change Requests
  - EX: Product Backlog Items

</details>

<!-- #endregion -->

<!-- #region Section 1.4.5 -->

## Roles in Testing [(1.4.5)](/Chapters/Chapter%201/Section_4.md#145)

<details>
  <summary>Roles in Testing Overview</summary>

- There are two (2) Principal Roles: **Test Management** and **Testing**
- Different people may take on these roles at different times.
  - Test Management Role can be performed by:
    - Team Leader
    - Test Manager
    - Development Manager
    - etc.
- One (1) person can also take on both roles at the same time.

</details>

<details>
  <summary>Test Management Role</summary>

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
  - Tasks for multiple teams or the entire organization may be performed by Test Managers outside of the Development Team

</details>

<details>
  <summary>Testing Role</summary>

- Overall responsible for:
  - Engineering (Technical) aspect of Testing
- Mainly focused on Activities of:
  - Test Analysis
  - Test Design
  - Test Implementation
  - Test Execution

</details>

<!-- #endregion -->

<!-- #region Section 1.5.2 -->

## Whole Team Approach [(1.5.2)](/Chapters/Chapter%201/Section_5.md#152)

<details>
  <summary>Whole Team Approach Overview</summary>

- Dependent on Context, Whole Team Approach is not always appropriate.
  - EX: Safety Critical, a high level of test independence may be needed.
- Any team member with the necessary knowledge or skills can perform any task.
- Whole team is responsible for Quality.

</details>

<details>
  <summary>Benefits of Whole Team Approach</summary>

- Improves team dynamics
- Enhances communication and collaboration
- Creates synergy

</details>

<!-- #endregion -->

<!-- #region Section 2.3 -->

## Maintenance Testing [(2.3)](/Chapters/Chapter%202/Section_3.md)

<details>
  <summary><strong>Maintenance Testing Overview</strong></summary>

  - Different Categories:
    - Corrective
    - Adaptive to changes in the environment
    - Improve performance or maintainability

</details>

<details>
  <summary><strong>Maintenance Testing Involves</strong></summary>

  - Planned Releases/Deployments
  - Unplanned Releases/Deployments (Hot Fixes)

</details>

<details>
  <summary><strong>Impact Analysis</strong></summary>

  - May be done before a change is made
  - Helps decide if the change is necessary

</details>

<details>
  <summary><strong>Production Change Testing</strong></summary>

  - Evaluates successful implementation
  - Checks for possible regressions on unchanged parts of the system

</details>

<details>
  <summary><strong>Scope Dependence</strong></summary>

  - Degree of risk of the change
  - Size of the existing system
  - Size of the change

</details>

<details>
  <summary><strong>Triggers for Maintenance Testing</strong></summary>

  - Modifications such as planned enhancements (Release-Based), corrective changes, or hot fixes
  - Upgrades or migrations of the operational environment
    - Can require tests associated with new environment, changes in software, or tests of data conversion
  - Retirement of a system
    - Testing of data archiving if long retention periods are required
    - Testing of restore and retrieval procedures after archiving

</details>

<!-- #endregion -->

<!-- #region Section 3.1.2 -->

## Value of Static Testing [(3.1.2)](/Chapters/Chapter%203/Section_1.md#312)

<details>
  <summary><strong>Value of Static Testing</strong></summary>

  - Can detect defects in the earliest phases of SDLC
  - Identify defects not found in Dynamic Testing
    - Unreachable Code
    - Design Patterns not implemented as desired
    - Defects in non-executable work products
  - Provides ability to evaluate the quality of Work Products
  - Provides build confidence in Work Products
  - Verifies documented requirements, so stakeholders can make sure requirements meet actual needs
  - Shared understanding between involved stakeholders
    - Should include a wide variety of stakeholders
  - Reviews may be more costly to implement, but overall project costs are much lower than with no reviews
    - Due to less time and effort necessary for fixing defects later
  - Code defects can be detected using Static Analysis more efficiently than Dynamic Testing
    - Fewer Code Defects
    - Lower overall Development effort

</details>

<!-- #endregion -->

<!-- #region Section 4.1 -->

## Test Techniques Overview [(4.1)](/Chapters/Chapter%204/Section_1.md)

<details>
  <summary><strong>Test Techniques Overview</strong></summary>

  - Supports tester in Test Analysis (what to test) and Test Design (how to test)
  - Helps to develop relatively small, but sufficient, set of test cases in a Systematic way
  - Helps tester _\_\_\_ during Test Analysis and Design:
    - Define Test Conditions
    - Identify coverage items
    - Identify Test Data

</details>

<details>
  <summary><strong>Black-Box Test Technique</strong></summary>

  - Referred to as Specification-Based Techniques
  - Based on analysis of the specified behavior of the test object without code knowledge
  - Test cases are independent of how the software is implemented
    - If there are code changes, but required behavior stays the same, test cases will stay useful

</details>

<details>
  <summary><strong>White-Box Test Techniques</strong></summary>

  - Referred to as Structure-Based Techniques
  - Based on analysis of the test object's internal structure and processing
  - Test cases are dependent on how the software is designed
    - Created only after design or implementation of the test object

</details>

<!-- #endregion -->

<!-- #region Section 4.2.1 -->

## Equivalence Partitioning [(4.2.1)](/Chapters/Chapter%204/Section_2.md#421)

<details>
  <summary><strong>Equivalence Partitioning</strong></summary>

  - Divides data into partitions
  - Partitions can be:
    - Continuous or discrete
    - Ordered or unordered
    - Finite or infinite
  - Theory:
    - If a test case tests one value from a partition and detects a defect
    - Then this defect should also be detected with other values within the same partition
    - Therefore one test for each partition is sufficient
  - Can be identified for any data element related to the test object:
    - Inputs
    - Outputs
    - Configuration items
    - Internal values
    - Time-Related values
    - Interface parameters
  - Simple test objects EP <u>CAN</u> be easy
    - In practice though, understanding how the test object will treat different values is often complicated
    - **Partitioning SHOULD BE done with care**
  - Coverage items are the Equivalence Partitions
  - Achieving 100% Coverage:
    - Test cases must exercise all identified partitions (includes invalid partitions) by covering each partition at least once
  - Coverage is measured by:
    - Number of partitions exercised by at least one test case
    - Divided by the total number of identified partitions
    - Coverage is expressed as a percentage
  - Many test objects include multiple sets of partitions
    - Test objects with more than one input parameter
    - Which means a test case will cover partitions from different sets of partitions
  - Each Choice Coverage
    - Simplest coverage criterion in the case of multiple sets of partitions
    - Each choice coverage requires test cases to exercise each partition from each set of partitions at least once
    - Each one does not take into account combinations of partitions

</details>

<details>
  <summary><strong>Valid Partition</strong></summary>

  - Partition containing valid values
    - Example - Valid values may be interpreted as those that should be processed by the test object or as those for which the specification defines their processing

</details>

<details>
  <summary><strong>Invalid Partition</strong></summary>

  - Partition containing invalid values
    - Example - Invalid values may be interpreted as those that should be ignored or rejected by the test object or as those for which no processing is defined in the test object specification
  - Definition of valid and invalid values dependent on team and organization

</details>

<!-- #endregion -->

<!-- #region Section 4.2.3 -->

## Decision Table Testing [(4.2.3)](/Chapters/Chapter%204/Section_2.md#423)

<details>
  <summary><strong>Decision Tables</strong></summary>

  - Used for testing implementation of system requirements that specify how different combinations of conditions result in different outcomes
  - Effective way of recording complex logic, such as business rules
  - Full decision table has enough columns to cover every combination of conditions  
  - Provides systematic approach to identify all combinations of conditions where some might be overlooked
  - Helps find any gaps or contradictions in the requirements
  - If there are many conditions:
    - Exercising all the decision rules may be time consuming:
      - Number of rules grows exponentially with the number of conditions
    - Reduce the number of rules that need to be exercised
    - Minimized decision table
    - Risk-Based approach

</details>

<details>
  <summary><strong>Decision Table can be simplified by</strong></summary>

- Deleting columns containing infeasible combinations of conditions
- Merging columns where conditions do not affect the outcome into a single column
- Minimization algorithms are out of scope of syllabus

</details>

<details>
  <summary><strong>Achieving 100% Coverage</strong></summary> 

- Test cases must exercise all these columns
- Number of exercised columns
- Divided by total number of feasible columns
- Expressed as a percentage

</details>

<details>
  <summary><strong>Decision Table Notation for Conditions</strong></summary> 

- **"T"** : True - Condition satisfied
- **"F"** : False - Condition is not satisfied
- **"-"** : Value of condition is irrelevant for action outcome
- **"N/A"** : Condition is infeasible for a given rule

</details>

<details>
  <summary><strong>Decision Table Notation for Actions</strong></summary> 

- **"X"** : Action should occur
- **"Blank"** : Action should not occur
- Other notations may be used

</details>

<details>
  <summary><strong>Decision Table Rows</strong></summary> 

- Conditions and resulting actions of the system are defined

</details>

<details>
  <summary><strong>Decision Table Columns</strong></summary> 

- Corresponds to a decision rule that defines a unique combination of conditions
- Along with associated actions

</details>

<details>
  <summary><strong>Limited-Entry Decision Table</strong></summary> 

- All values of the conditions and actions (except for irrelevant or infeasible ones) are shown as Boolean values (True or False)

</details>

<details>
  <summary><strong>Extended-Entry Decision Table</strong></summary> 

- Some or all conditions or actions may take on multiple values:
  - Ranges of numbers
  - Equivalence partitions
  - Discrete Values

</details>

<!-- #endregion -->

<!-- #region Section 4.2.4 -->

## State Transition Testing [(4.2.4)](/Chapters/Chapter%204/Section_2.md#424)

<details>
  <summary><strong>State Transition Testing</strong></summary>

  - Test case based on a State Transition Diagram or Stable Table is usually represented as a sequence of events:
    - Results in a sequence of state changes (and actions if necessary)
  - One test case may, and usually will, cover several transitions between states
  - There are many coverage criteria for state transition testing

</details>

<details>
  <summary><strong>State Transition Diagram</strong></summary>

- Models the behavior of a system by showing its possible states and valid state transitions
- Transition is initiated by an event:
  - May be additionally qualified by a guard condition
- Transitions are assumed to be instantaneous and may sometimes result in the software taking action
- Common Transition Labeling:
  - "Event [guard condition] / Action"
- Guard conditions and actions can be omitted if they do not exist or are irrelevant for the tester

</details>

<details>
  <summary><strong>Stable Table</strong></summary>

- Equivalent Model to State Transition Diagram
- In contrast to Transition Diagram, State Table explicitly shows invalid transitions:
  - Represented by empty cells

</details>

<details>
  <summary><strong>Stable Table Rows</strong></summary>

- Represent states

</details>

<details>
  <summary><strong>Stable Table Columns</strong></summary>

- Represent events (together with guard conditions if they exist)

</details>

<details>
  <summary><strong>Stable Table Entries (Cells)</strong></summary>

- Represent transitions and contain:
  - Target State
  - Resulting Actions, if defined

</details>

<details>
  <summary><strong>All States Coverage</strong></summary>

- Coverage items are the states
- Achieving 100% Coverage:
  - Test cases must ensure all states are visited
  - Number of visited states
  - Divided by the total number of states
  - Expressed as a percentage
</details>

<details>
  <summary><strong>Valid Transitions Coverage</strong></summary>

- Also called 0-Switch Coverage
- Coverage items are single valid transitions
- Achieving 100% Coverage:
  - Test cases must exercise all the valid transitions
  - Number of exercised valid transitions
  - Divided by the total number of valid transitions
  - Expressed as a percentage

</details>

<details>
  <summary><strong>All Transitions Coverage</strong></summary>

- Coverage items are all transitions shown in a State Table
- Testing only one invalid transition in a single test case helps to avoid fault masking:
  - Situation in which one defect prevents the detection of another
- Achieving 100% Coverage:
  - Test cases must exercise all the valid transitions and attempt to execute invalid transitions
  - Number of valid and invalid transitions exercised or attempted to be covered by executed test cases
  - Divided by the total number of valid and invalid transitions
  - Expressed as a percentage

</details>

<details>
  <summary><strong>Coverage</strong></summary>

- **Valid Transitions** is the most widely used coverage criterion
- **All States Coverage** is weaker than **Valid Transitions Coverage**:
  - Due to it typically being able to achieve without exercising all the transitions
- Achieving full **Valid Transition Coverage** guarantees full **All States Coverage**
- Achieving full **All Transitions Coverage** guarantees both full **All States Coverage** and full **Valid Transitions Coverage**:
  - Should be a minimum requirement for mission and safety-critical software

</details>

<!-- #endregion -->

<!-- #region Section 4.3.1 -->

## Statement Testing and Statement Coverage [(4.3.1)](/Chapters/Chapter%204/Section_3.md#431)

<details>
  <summary><strong>Statement Testing and Statement Coverage</strong></summary>

  - **Statement Testing**
    - Coverage items are executable statements
    - Design test cases that exercise statements in the code until an acceptable level of coverage is achieved
    - Coverage is measured as:
      - The number of statements exercised by the test cases
      - Divided by the total number of executable statements in the code
      - Expressed as a percentage
    - When 100% coverage is achieved:
      - Ensures all executable statements in the code have been tested at least once
      - Each statement with a defect has been executed:
        - May cause failure in detecting the presence of defect
      - Exercising a statement with a test case will not detect defects in **ALL** cases:
        - Data Dependent statements:
          - Division by zero
      - 100% Coverage does not guarantee all decision logics have been tested:
        - May not exercise all branches

</details>

<!-- #endregion -->

<!-- #region Section 4.3.2 -->

## Branch Testing and Branch Coverage [(4.3.2)](/Chapters/Chapter%204/Section_3.md#432)

<details>
  <summary><strong>Branch Testing and Branch Coverage</strong></summary>

  - **Branch**
    - Transfer of control between 2 nodes in control graph
    - Shows possible sequences in which source code statements are executed in the test object
    - Transfer of control can be:
      - Unconditional (Straight-Line Code)
      - Conditional (Decision outcome)

  - **Branch Testing**
    - Coverage items are branches
    - Design test cases to exercise branches in the code until an acceptable level of coverage is achieved
    - Coverage is measured as:
      - Number of branches exercised by the test cases
      - Divided by the total number of branches
      - Expressed as a percentage

  - **100% Branch Coverage**
    - All branches in the code, unconditional and conditional, are exercised by test cases
    - Conditional branches typically correspond to a true or false outcome:
      - "If...Then" Decision
      - A Switch/Case Statement
      - Decision to exit or continue loop
    - Exercising a branch with a test case will not detect defects in all cases:
      - May not detect defects requiring the execution of a specific path in the code
    - Branch coverage subsumes statement coverage:
      - Any set of test cases achieving 100% **Branch Coverage** also achieves 100% **Statement Coverage**, but not vice versa

</details>

<!-- #endregion -->

<!-- #region Section 4.3.3 -->

## The Value of White-Box Testing [(4.3.3)](/Chapters/Chapter%204/Section_3.md#433)

<details>
  <summary><strong>The Value of White-Box Testing</strong></summary>

  - **Fundamental Strength**
    - Entire software implementation is taken into account during testing
    - Facilitates defect detection even when software specification is vague, outdated, or incomplete

  - **Weakness**
    - If the software does not implement one or more requirements, White-Box Testing may not detect the resulting defects of omission

  - Can be used in Static Testing
    - During dry runs of code

  - Well suited to reviewing code that is not yet ready for:
    - Execution
    - Pseudocode
    - High-Level or Top-Down Logic which can be modeled with a control flow graph

  - Only Black-Box Testing does not provide a measure of actual code coverage
  - White-Box Coverage measures provide an objective measurement of coverage:
    - Provides the necessary information to allow additional tests to be generated for:
      - Increase of coverage
      - Increase of confidence in the code

</details>

<!-- #endregion -->

<!-- #region Section 4.4.1 -->

## Error Guessing [(4.4.1)](/Chapters/Chapter%204/Section_4.md#441)

<details>
  <summary><strong>Error Guessing</strong></summary>

  - Used to anticipate the occurrence of errors, defects, and failures based on tester's knowledge:
    - How the application has worked in the past
    - Type of errors developers tend to make
    - Type of defects from errors
    - Types of failures that have occurred in other, similar applications

  - Generally, errors, defects, and failures may be related to:
    - **Input**
      - Correct input not accepted
      - Parameters wrong or missing
    - **Output**
      - Wrong format
      - Wrong result
    - **Logic**
      - Missing cases
      - Wrong operator
    - **Computation**
      - Incorrect operand
      - Wrong computation
    - **Interfaces**
      - Parameter mismatch
      - Incompatible types
    - **Data**
      - Incorrect initialization
      - Wrong type
  
  - Fault attacks are a methodical approach to the implementation of error guessing
  - Technique requires tester to create or acquire a list of possible:
    - Errors
    - Defects
    - Failures

    - The list will help:
      - Identify defects associated with the errors
      - Expose the defects
      - Cause the failures

    - List can be built based on:
      - Experience 
      - Defect and Failure data
      - Common knowledge about why software fails

</details>


<!-- #endregion -->

<!-- #region Section 5.1.3 -->

## Entry Criteria and Exit Criteria [(5.1.3)](/Chapters/Chapter%205/Section_1.md#513)

<details>
  <summary><strong>Entry Criteria and Exit Criteria</strong></summary>

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
      - **Availability of Resources**
        - People
        - Tools
        - Environments
        - Test Data
        - Budget
        - Time
      - **Availability of Software**
        - Test Basis
        - Testable Requirements
        - User Stories
        - Test Cases
      - **Initial Quality Level of a Test Object**
        - All Smoke Tests have passed
        
  - **Exit Criteria**
    - Defines what must be achieved in order to declare an activity completed
    - Typical Exit Criteria:
      - **Measures of Thoroughness**
        - Achieved level of Coverage
        - Number of Unresolved Defects
        - Defect Density
        - Number of Failed Test Cases
      - **Completion Criteria**
        - Planned Tests have been executed
        - Static Testing has be performed
        - All defects found are reported
        - All Regression Tests are automated
      - **Running out of time or budget**
    - If stakeholders have reviewed and accepted the risks to go live, all Exit Criteria do not need to be satisfied

  - **Agile Software Development**
    - Exit Criteria is known as **Definition of Done**
      - Defines the team's objective metrics for a releasable item
    - Entry Criteria is known as **Definition of Ready**
      - Criteria that must be fulfilled to start the development and/or testing activities

</details>

<!-- #endregion -->

<!-- #region Section 5.1.4 -->

## Estimation Techniques [(5.1.4)](/Chapters/Chapter%205/Section_1.md#514)

<details>
  <summary><strong>Estimation Techniques</strong></summary>

  - **Estimation Overview**
    - Predicting the amount of test-related work needed to meet the objectives of a test project
    - Important to clarify to stakeholders that the estimate is based on several assumptions and is subject to estimation error
    - Estimation for small tasks is usually more accurate than for large tasks
    - For large tasks, decompose into smaller tasks and estimate those

  - **Estimation based on Ratios**
    - **Metrics-Based Technique**
      - Figures collected from previous projects within the organization
        - Allows deriving "standard" ratios for similar projects
      - Best source for estimation is historical data from the organization
        - Example:
          - Previous Project Development-to-Test Effort ratio was 3:2
          - Current Project Development Effort is 600 person-days
          - Test Estimate = 400 person-days
            - Calculation: 600 / 3 = 200, 200 * 2 = 400

  - **Extrapolation**
    - **Metrics-Based Technique**
      - Measurements are made early in the project to gather data
      - Effort required for the remaining work is approximated by extrapolating this data
        - Usually with a mathematical model
      - Suitable for Iterative SDLCs
        - Example:
          - Extrapolate test effort for the next iteration as the average effort from the last three iterations

  - **Wideband Delphi**
    - **Iterative, Expert-Based Technique**
      - Experts make experience-based estimations
      - Experts estimate effort in isolation
      - Results are collected, and if deviations are out of agreed boundaries, experts discuss and re-estimate
      - Repeated until consensus is achieved

    - **Planning Poker**
      - Variant of Wideband Delphi
      - Commonly used in Agile Software Development
      - Estimates made using cards with numbers representing effort size

  - **Three-Point Estimation**
    - **Expert-Based Technique**
      - Estimation is based on a single test case
      - Experts provide three estimations:
        - Most Optimistic (A)
        - Most Likely (M)
        - Most Pessimistic (B)
      - Final Estimate (E) = (A + 4*M + B) / 6
      - Allows calculation of measurement error
        - SD = (B - A) / 6

    - **Example:**
      - A = 6
      - M = 9
      - B = 18
      - Estimation:
        - E = (6 + (4 * 9) + 18) / 6 = 10
        - For 4 test cases: E = 10 * 4 = 40
      - Measurement Error:
        - SD = (18 - 6) / 6 = 2
      - Final Answer:
        - 10 ± 2

</details>


<!-- #endregion -->

<!-- #region Section 5.1.5 -->

## Test Case Prioritization [(5.1.5)](/Chapters/Chapter%205/Section_1.md#515)

<details>
  <summary><strong>(5.1.5) Test Case Prioritization</strong></summary>

  - Test Cases and Test procedures are specified and assembled into Test Suites
    - Test Suites are then arranged in a Test Execution Schedule
      - Defined by the order they are to be run

  - Different factors are taken into account
  - Most commonly used Test Case Prioritization Strategies:
    - **Risk-Based Prioritization**
      - Order of Test Execution is based on results of [Risk Analysis](Section_2.md#523)
      - Test Cases covering the most important risks are executed first

    - **Coverage-Based Prioritization**
      - Order of Test Execution is based on Coverage (Statement Coverage)
      - Test Cases achieving the highest coverage are executed first
      - **Additional Coverage Prioritization**
        - Another variant of Coverage-Based Prioritization
        - Test Case achieving the highest coverage is executed first
        - Each subsequent test case is the one that achieves the highest additional coverage

    - **Requirements-Based Prioritization**
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

</details>


<!-- #endregion -->

<!-- #region Section 5.1.7 -->

## Testing Quadrants [(5.1.7)](/Chapters/Chapter%205/Section_1.md#517)

<details>
  <summary><strong>(5.1.7) Testing Quadrants</strong></summary>

  - With Agile, Testing Quadrants are grouped by the test levels with the appropriate:
    - Test Types
    - Activities
    - Test Techniques
    - Work Products

  - Model supports test management in visualizing this
    - Ensures that all appropriate test types and test levels are included in the SDLC
    - Understands that some test types are more relevant to certain test levels than others
    - Provides a way to differentiate and describe the types of tests to:
      - All Stakeholders
      - Developers
      - Testers
      - Business Representatives

  - Tests can be Business Facing or Technology Facing
  - Tests support the team (Guide the development) or critique the product (Measure its behavior against the expectations)
    - These two viewpoints determine the four quadrants:

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
      - Tests are often automated

</details>


<!-- #endregion -->

<!-- #region Section 5.2.1 -->

## Risk Definition and Risk Attributes [(5.2.1)](/Chapters/Chapter%205/Section_2.md#521)

<details>
  <summary><strong>(5.2.1) Risk Definition and Risk Attributes</strong></summary>

  - Risk is a potential **Event** whose occurrence causes an adverse effect:
    - Event
    - Hazard
    - Threat
    - Situation

  - Risk can be characterized by two factors:
    - **Risk Likelihood**
      - Probability of Risk Occurrence (greater than 0, less than 1)
    - **Risk Impact (Harm)**
      - Consequences of this occurrence
    - These factors express the risk level
      - Measure for the risk
      - Higher the risk level, the more important is its treatment
    - **Risk Level = Risk Impact * Risk Likelihood**

</details>


<!-- #endregion -->

<!-- #region Section 5.3.2 -->

## Purpose, Content, and Audience for Test Reports [(5.3.2)](/Chapters/Chapter%205/Section_3.md#532)

<details>
  <summary><strong>(5.3.2) Purpose, Content, and Audience for Test Reports</strong></summary>

  - **Test Reporting** summarizes and communicates test information during and after testing

  - **Test Progress Reports** support the ongoing control of the testing
    - When changes are needed due to deviation from the plan or changed circumstances, report must provide enough information to make modifications to:
      - Test Schedule
      - Resources
      - Test Plan

  - **Test Completion Reports**
    - Summarize a specific stage of testing and can give information for subsequent testing
      - Test Level
      - Test Cycle
      - Iteration
    - Prepared during test completion, when a **Test Level** is complete:
      - Project
      - Test level
      - Test type
    - Or ideally, the exit criteria have been met
    - Report uses test progress reports and other data
    - Typically includes:
      - Test Summary
      - Testing and Product quality evaluation based on the original test plan
        - Test Objectives
        - Exit Criteria
      - Deviations from the test plan
        - Differences from the planned schedule, duration, and effort
      - Testing impediments and workarounds
      - Test metrics based on test progress reports
      - Unmitigated risks, defects not fixed
      - Lessons learned that are relevant to the testing
  
  - During Test Monitoring and Control, test team generates test progress reports for stakeholders to keep them informed
  - Test Reports are usually generated on a regular basis and include:
    - Test Period
    - Test Progress including any notable deviations
      - Ahead or behind schedule
    - Impediments for testing and their workarounds
    - [Test Metrics](#531)
    - New and changed risks within the testing period
    - Testing planned for the next period

  - Different audiences:
    - Require different information in the reports
    - Influence the degree of formality
    - The frequency of reporting
  
  - Test Progress Reporting to others in the same team is often frequent and informal
  - Project Testing Completion Reporting follows a set template and occurs only once

  - Test Completion Reports and Test Progress Reports (Test Status Reports) templates and examples can be found at ISO/IEC/IEEE 29119-3

</details>


<!-- #endregion -->

<!-- #region Section 5.5 -->

## Defect Management [(5.5)](/Chapters/Chapter%205/Section_5.md)

<details>
  <summary><strong>Defect Management</strong></summary>

  - A major test objective is to find defects, therefore an established Defect Management Process is essential
  - Reported anomalies may turn out to be real defects or something else
    - False positive
    - Change request
  - These defects are resolved during the process of dealing with defect reports
  - Anomalies may be reported during any phase of the SDLC and the form depends on the SDLC
  - At a minimum, Defect Management Process includes a workflow for handling individual anomalies from their discovery to their closure and rules for their classification
  - Workflow typically comprises activities to:
    - Log the reported anomalies
    - Analyze anomalies
    - Classify anomalies
    - Decide on a suitable response
      - Fix anomalies
      - Keep as is
    - Close the defect report

  - Typical defect reports have the following objectives:
    - Provide those responsible for handling and resolving reported defects with sufficient information to resolve the issue
    - Provide a means of tracking the quality of the work product
    - Provide ideas for improvement of the development and test process

  - A defect report logged during dynamic testing typically includes:
    - Unique identifier
    - Title with a short summary of the anomaly being reported
    - Date when the anomaly was observed, issuing organization, and author, including their role
    - Identification of the test object and test environment
    - Context of the defect
      - Test case being run
      - Test activity being performed
      - SDLC phase
      - Other relevant information such as:
        - Test technique
        - Checklist
        - Test data being used
    - Description of the failure to enable reproduction and resolution including the steps that detected the anomaly, and any relevant **test logs**, **database dumps**, **screenshots**, or **recordings**
    - Expected/Actual Results
    - Severity of defect on the interests of stakeholders or requirements
    - Priority to fix
    - Status of the defect
      - Open
      - Deferred
      - Duplicate
      - Waiting to be fixed
      - Awaiting confirmation of testing
      - Re-opened
      - Closed
      - Rejected
    - References
      - to the test cases

  - Some of the listed data may automatically included when using defect management tools
    - Identifier
    - Date
    - Author
    - Initial Status

  - Document templates for a defect report and example defect reports can be found in ISO/IEC/IEEE 29119-3 Standard

</details>


<!-- #endregion -->

<!-- #region Section 6.2 -->

## Benefits and Risks of Test Automation [(6.2)](/Chapters/Chapter%206/Section_2.md)

<details>
  <summary><strong>Benefits and Risks of Test Automation</strong></summary>

  - Acquiring a tool does not guarantee success
    - Each new tool will require effort to achieve real and lasting benefits
      - Tool introduction
      - Tool maintenance
      - Tool training
    - Some risks need analysis and mitigation

  - **Test Automation Benefits:**
    - Time saved by reducing repetitive manual work
      - Execute regression tests
      - Re-enter the same test data
      - Compare expected vs actual results
      - Check against coding standards
    - Prevention of simple human errors through greater consistency and repeatability
      - Tests are consistently derived from requirements
      - Test data is created in a systematic manner
      - Tests are executed by a tool in the same order with the same frequency
    - More objective assessment (coverage) and providing measures that are too complicated for humans to derive
    - Easier access to information about testing to support test management and test reporting
      - Statistics
      - Graphs
      - Aggregated data about test progress
      - Defect rates
      - Test execution duration
    - Reduced test execution times to provide earlier defect detection, faster feedback, and faster time to market
    - More time for testers to design new, deeper, and more effective tests

  - **Test Automation Risks:**
    - Unrealistic expectations about the benefits of a tool
      - Functionality
      - Ease of use
    - Inaccurate estimations of time, costs, and effort required to introduce a tool, maintain test scripts, and change the existing manual test process
    - Using a test tool when manual testing is more appropriate
    - Relying on a tool too much
      - Ignoring the need for human critical thinking
    - The dependency on the tool vendor which may:
      - Go out of business
      - Retire the tool
      - Sell the tool to a different vendor
      - Provide poor support
        - Responses to queries
        - Upgrades
        - Defect fixes
    - Using open-source software which may be abandoned, leading to no further updates, or requiring frequent updates due to further development
    - The automation tool is not compatible with the development platform
    - Choosing an unsuitable tool that does not comply with regulatory requirements and/or safety standards

</details>


<!-- #endregion -->