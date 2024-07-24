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
    - K3: Apply - You should be able to select the correct application of a concept or technique and apply it to a given context

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