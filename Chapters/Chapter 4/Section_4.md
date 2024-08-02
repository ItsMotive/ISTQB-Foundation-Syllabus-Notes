<details>
  <summary>Table of Contents</summary>
  <ul>
    <li><a href="/README.md">Home</a></li>
    <li><a href="Chapter_4_Home.md">Chapter Home</a></li>
    <li><a href="Section_1.md">Section 1</a></li>
    <li><a href="Section_2.md">Section 2</a></li>
    <li><a href="Section_3.md">Section 3</a></li>
    <li><a href="Section_4.md">Section 4</a></li>
    <li><a href="Section_5.md">Section 5</a></li>
  </ul>
</details>

# Section Guide
- [(K2) Explain error guessing](#441)
- [(K2) Explain exploratory testing](#442)
- [(K2) Explain checklist-based testing](#443)

<a id=44></a>

## (4.4) Experience-Based Test Techniques
- Commonly used techniques:
  - Error Guessing
  - Exploratory Testing
  - Checklist-Based Testing

  <a id=441></a>
  
  ## (4.4.1) Error Guessing
  - Used to anticipate the occurrence of errors, defects, and failures, based on tester's knowledge:
    - How the application has worked in the past
    - Type of errors developers tend to make
    - Type of defects from errors
    - Types of failures that have occurred in other, similar applications

  - Generally, errors, defects, and failures may be related to:
    - Input
      - Correct input not accepted
      - Parameters wrong or missing
    - Output
      - Wrong format
      - Wrong result
    - Logic
      - Missing cases
      - Wrong operator
    - Computation
      - Incorrect operand
      - Wrong computation
    - Interfaces
      - Parameter mismatch
      - Incompatible types
    - Data
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

  <a id=442></a>

  ## (4.4.2) Exploratory Testing
  
  - Tests are simultaneously \_\_\_\_ while tester learns about test object:
    - Designed
    - Executed
    - Evaluated

  - Used to: 
    - Learn more about test object
    - Explore it more deeply with focused tests
    - Create tests for untested areas

  - Useful when:
    - There are few or inadequate specifications
    - There is significant time pressure on testing
    - Trying to complement other more formal test techniques

  - More effective when tester:
    - Is experienced
    - Has domain knowledge
    - Has high degree of [essential skills](/Chapters/Chapter%201/Section_5.md#151)
      - Analytical skills
      - Curiosity
      - Creativeness

  - Can incorporate other test techniques

  - **Session-Based Testing**
    - Exploratory Testing is conducted based of this to structure the testing
    - With this approach, Exploratory Testing is conducted within a defined Time-Box
    - Tester uses a Test Charter containing Test Objectives to guide the testing
    - Test session is usually followed by a debriefing 
      - Discussion between tester and stakeholders interested in the test results of the test session
    - Test objectives are treated as high-level test conditions
    - Coverage items are identified and exercised during test session
    - Testers use test session sheets to:
      - Document the steps followed
      - Document the discoveries made

  <a id=443></a>

  ## (4.4.3) Checklist-Based Testing
  - Tester \_\_\_\_ to cover test conditions from a checklist:
    - Designs
    - Implements
    - Execute tests

  - In the absence of detailed test cases, Checklist-Based Testing can:
    - Provide guidelines
    - Some degree of consistency for testing
  
  - **Checklists** 
    - Can be built based on:
      - Experience 
      - Knowledge about what is important for the user
      - Understanding of why and how software fails

    - Can be created to support:
      - Various test types
        - Functional
        - Non-Functional

    - Should be regularly updated based on defect analysis
      - Care should be taken to avoid letting checklist being too long

    - Should not contain items that can be checked automatically
    - Entry/Exit Criteria or items too general are better suited
    - If this is high-level, some variability in actual testing is likely to occur
      - Results in potentially greater coverage
      - Less Repeatability

  - **Checklist Items**
    - Often phrased in the form of a question
    - Should be possible to check each item separately and directly

    - Items may refer to:
      - Requirements
      - Graphical interface properties
      - Quality characteristics
      - Other forms of test conditions

    - May gradually become less effective over time
      - Due to developers learning to avoid making the same errors
    
    - New entries may also need to be added to reflect newly found high severity defects