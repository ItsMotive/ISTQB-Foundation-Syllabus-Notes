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

- [(K2) Explain statement testing](#431)
- [(K2) Explain branch testing](#432)
- [(K2) Explain the value of white-box testing](#433)

## (4.3) White-Box Test Techniques

- Popular and Simple
- Focuses on two code-related white-box test techniques:
  - Statement Testing
  - Branch Testing
- More rigorous techniques are used in \_\_\_\_ to achieve more thorough code coverage:

  - Safety-Critical Environments
  - Mission-Critical Environments
  - High-Integrity Environments

  <a id="431"></a>

  ## (4.3.1) Statement Testing and Statement Coverage

  - **Statement Testing**
    - Coverage items are executable statements
    - Design test cases that exercise statements in the code until an acceptable level of coverage is achieved
    - Coverage is measured as:
      - The number of statements exercised by the test cases
      - Divided by the total number of executable statements in the code
      - Expressed as a percentage
    - When 100% coverage is achieved:
      - Ensures all executable statements in the code has been tested at least once
      - Each statement with a defect has been executed
        - May cause failure in detecting presence of defect
      - Exercising a statement with a test case will not detect defects in **ALL** cases
        - Data Dependent statements
          - Division by zero
      - 100% Coverage does not guarantee all decision logics have been tested
        - May not exercise all branches

  <a id="432"></a>

  ## Branch Testing and Branch Coverage

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
    - Conditional branches typically correspond to a true of false outcome
      - "If...Then" Decision
      - A Switch/Case Statement
      - Decision to exit or continue loop
    - Exercising a branch with a test case will not detect defects in all cases
      - May not detect defects requiring the execution of a specific path in a code
  - Branch coverage subsumes statement coverage
    - Any set of test cases achieving 100% **Branch Coverage** also achieves 100% **Statement Coverage**, not vise versa

  <a id=433></a>

  ## The Value of White-Box Testing
  - Fundamental Strength
    - Entire software implementation is taken into account during testing
    - Facilitates defect detection even when software specification is vague, outdated, or incomplete

  - Weakness
    - If the software does not implement one or more requirements, White-Box Testing may not detect the resulting defects of omission

  - Can be used in Static Testing
    - During dry runs of code

  - Well suited to reviewing code that is not yet ready for:
    - Execution
    - Pseudocode
    - High-Level or Top-Down Logic which can be modeled with a control flow graph

  - Only Black-Box Testing does not provide a measure of actual code coverage
  - White-Box Coverage measures provide an objective measurement of coverage
    - Provides the necessary information to allow additional tests to be generated for:
      - Increase of coverage
      - Increase of confidence in the code