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

  <a id=431></a>

  ## Statement Testing and Statement Coverage

  - Popular and Simple
  - Code-Related White-Box Test Techniques:
    - Statement Testing
    - Branch Testing
  - More rigorous testing techniques are used in \_\_\_\_ for more thorough code coverage
    - Safety-Critical Environments
    - Mission-Critical Environments
    - High-Integrity Environments

  <a id=431></a>

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

  <a id=432></a>

  ## Branch Testing and Branch Coverage

  - **Branch**
    - Transfer of control between 2 nodes in control graph
    - Shows possible sequences in which source code statements are executed in the test object
    - Transfer of control can be:
      - Unconditional (Straight-Line Code)
      - Conditional (Decision outcome)
  - **Branch Testing**
    - Coverage items are branches
    -
