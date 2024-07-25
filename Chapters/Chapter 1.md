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
- [What is Testing?](#what-is-testing?)
    - [(K1) Identify Typical Test Objectives](#Test-Objectives)
    - [(K2) Differentiate Testing from Debugging](#testing-and-debugging)
- [Why is Testing Necessary?]()
    - [(K2) Exemplify Why Testing is Necessary]()
    - [(K1) Recall the Relation between Testing and Quality Assurance]()
    - [(K2) Distinguish between Root Cause, Error, Defect, and Failure]()
- [Testing Principles]()
    - [(K2) Explain the Seven Testing Principles]()
- [Test Activities, Testware, and Test Roles]()
    - [(K2) Summarize the Different Test Activities and Tasks]()
    - [(K2) Explain the Impact of Context on the Test Process]()
    - [(K2) Differentiate the Testware that Supports the Test Activities]()
    - [(K2) Explain the Value of Maintaining Traceability]()
    - [(K2) Compare the Different Roles in Testing]()
- [Essential Skills and Good Practices in Testing]()
    - [(K2) Give Examples of the Generic Skills Required for Testing]()
    - [(K1) Recall the Advantages of the Whole Team Approach]()
    - [(K2) Distinguish the Benefits and Drawbacks of Independence of Testing]()

## What is Testing?

**Software Testing...**
- Assesses Software Quality and helps reducing the risk of software failure.
- Set of activities to find defects and evaluate the quality of software artifacts.
- May be [Static](Chapter%203.md) or [Dynamic](Chapter%204.md).
- Is technical and needs to be properly [Planned, Managed, Estimated, Monitored, and Controlled](Chapter%205.md).
- Is an intellectual activity, requiring testers to have specialized knowledge, use analytical skills, and apply critical thinking and systems thinking. 
- Uses [Tools](Chapter%206.md)

    ## Test Objectives
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

    ## Testing and Debugging
    - **Testing:** Triggers failure that are caused by defects in the software or finds defects in the test object.

    - **Debugging:** Finds causes for defect/failure, analyzes, and eliminates them.

    - **Debugging Process:**
        - Reproduction of a failure
        - Diagnosis (Finding Root Cause)
        - Fixing the cause

    - **Subsequent Confirmation Testing** - Initial Tester checks whether the fixes resolved the problem.
    - **Subsequent Regression Testing** - Checks whether the fixes are causing failures in other parts of the test object. [(Section 2.2.3)](Chapter%202.md#Distinguish-confirmation-testing-from-regression-testing)
    - With Static Testing, there is no need for reproduction or diagnosis, since it directly finds defects and cannot cause failures. 

## Why is Testing necessary?
- Testing components, systems, and associated documentation helps to identify defects in software.
- Testing's contribution to success should not be restricted to the test team's activities.

- **Testing:**
    - Helps achieve agreed upon goals within:
        - Set Scope
        - Time
        - Quality
        - Budget Constraint

    ## Testing's Contributions to Success
    - Testing indirectly contributes to high quality test objects.
    - Test objects contribute to decisions to move to next stages of SDLC, such as release decision.

    - **Testing Provides:**
        - Cost-Effective means of detecting defects
        - Means of directly evaluating the quality of a test object at various stages in the SDLC
        - Users with indirect representation on the development project
        - Means of meeting contractual or legal requirements
        - Means of complying with regulatory standards

    ## Testing and Quality Assurance (QA)
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

    ## Errors, Defects, Failures, and Root Causes
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

## Testing Principles
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
    - [Test Case Prioritization](Chapter%205#Section-5.1.5)
    - [Risk-Based Testing](Chapter%205#Section-5.2)

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
    - Create new testse
- Repeating tests such as Automated Regression **can** be beneficial

### 6. Testing is context dependent.
- No universally correct approach to testing.

### 7. Absence-of-Defects Fallacy.
- It is a misconception that software verification will result in the success of a system.
- Even testing all specified requirements and fixing all defects found, it does not guarantee:
    - System fulfills users' needs and expectations
    - Achieve customer's business goals
- Verification and Validation should both be done.