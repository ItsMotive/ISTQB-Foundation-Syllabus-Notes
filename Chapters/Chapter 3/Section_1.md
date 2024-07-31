<details>
  <summary>Table of Contents</summary>
  <ul>
    <li><a href="/README.md">Home</a></li>
    <li><a href="Chapter_3_Home.md">Chapter Home</a></li>
    <li><a href="Section_1.md">Section 1</a></li>
    <li><a href="Section_2.md">Section 2</a></li>
  </ul>
</details>

# Section Guide

- [Recognize types of products that can be examined by the different static test techniques](Section_1.md#311)
- [Explain the value of static testing](Section_1.md#312)
- [Compare and contrast static and dynamic testing](Section_1.md#313)

<a id=31></a>

## Static Testing Basics
- Testing software without executing the code
- Can be applied for verifications and validations
- Cab identify problems prior to dynamic testing due to:
    - Requiring less effort
    - No test cases are required
    - [Tools](/Chapters/Chapter%206/Chapter_6_Home.md) are typically used
- **Static Analysis**
    - Evaluates maintainability and security
    - Tools:
        - Spelling Checkers
        - Readability Tools
- Tools:
    - Static Analysis
- Manual Examinations/Reviews:
    - Code
    - Process Specification
    - System Architecture Specification
    - Other Work Products
- Test Objectives:
    - Improving Quality
    - Detecting Defects
    - Assessing Characteristics like:
        - Readability
        - Completeness
        - Correctness
        - Testability
        - Consistency
- To ensure User Stories and related Work Products meet Defined Criteria ([Definition of Ready](/Chapters/Chapter%205/Section_1.md#513)):
    - Participants:
        - Testers
        - Business Representatives
        - Developers
    - Work together on:
        - Example Mappings
        - Collaborative User Story Writing
        - Backlog Refinement Sessions
- Review techniques can be applied to ensure user stories are:
    - Complete
    - Understandable
    - Include Testable Acceptance Criteria
- Improving Proposed User Stories can be done by:
    - Asking the right questions
    - Testers explore and challenge

    <a id=311></a>

    ## (3.1.1) Work Products Examinable by Static Testing
    - Almost any Work Product can be examined using Static Testing
        - Requirement Specification Documents
        - Source Code
        - Test Plans
        - Test Cases
        - Product Backlog Items
        - Test Charters
        - Project Documentation
        - Contracts
        - Models
    - Even though any Work Product that can be read and understood can be a subject of a review, Static Testing requires a structure to be compared to:
        - Models
        - Codes
        - Text with a formal syntax
    - Work Products not appropriate for Static Testing:
        - Difficult to interpret by human beings
        - Should not be analyzed by tools

    <a id=312></a>

    ## (3.1.2) Value of Static Testing
    - Can detect defects in the earliest phases of SDLC
    - Identify defects not found in Dynamic Testing
        - Unreachable Code
        - Design Patterns not implemented as desired
        - Defects in non-executable work products
    - Provides ability to evaluate the quality of Work Products
    - Provides build confidence in Work Products
    - Verifies documented requirements, so stakeholders can make sure requirements meet actual needs
    - Shared understanding between involved stakeholders
        - Should include wide variety of stakeholder
    - Reviews may be more costly to implement, but overall project costs are much lower than with no reviews
        - Due to less time and effort necessary for fixing defects later
    - Code defects can be detected using Static Analysis more efficiently than Dynamic Testing
        - Fewer Code Defects
        - Lower overall Development effort

    <a id=313></a>

    ## (3.1.3) Differences between Static Testing and Dynamic Testing
    - Both testing practices complement each other
    - They have similar objectives:
        - Supporting the detection of defects in Work Products
    - Differences:
        - Some defect types can only be found by Static or Dynamic Testing
        - Static Testing find defects directly, while Dynamic Testing causes failures from associated defects are determined through subsequent analysis
        - Static Testing may more easily detect defects in the code, where they aren't executed or hard to reach during Dynamic Testing
        - Static Testing can be applied to non-executable Work Products, while Dynamic Testing can only be applied to executable Work Products
        - Static Testing can be used to measure quality characteristics that are not dependent on executing code (Maintainability), while Dynamic Testing can be used to measure quality characteristics that are dependent on executing code (Performance Efficiency)
    - Easier/Cheaper defects found through Static Testing:
        - Defects in requirements
            - Inconsistencies
            - Ambiguities
            - Contradictions
            - Omissions
            - Inaccuracies
            - Duplications
        - Design defects
            - Inefficient Database Structures
            - Poor Modularization
        - Certain Types of Coding Defects
            - Variables with undefined values
            - Undeclared variables
            - Unreachable code
            - Duplicated code
            - Excessive code complexity
        - Deviations from Standards
            - Lack of adherence to naming conventions in coding standards
        - Incorrect Interface Specifications
            - Mismatched number
            - Type of parameters
            - Order of parameters
        - Specific types of Security Vulnerabilities
            - Buffer Overflows
        - Gaps or Inaccuracies in Test Basis Coverage
            - Missing Tests for an Acceptance Criterion