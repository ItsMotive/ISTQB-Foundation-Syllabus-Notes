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

- [(K2) (1.3.1) Explain the Seven Testing Principles](#13)

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
- Instead use \_\_\_\_ to focus test efforts:
  - [Test Techniques](/Chapters/Chapter%204/Chapter_4_Home.md)
  - [Test Case Prioritization](/Chapters/Chapter%205/Section_1.md#515)
  - [Risk-Based Testing](/Chapters/Chapter%205/Section_2.md#52)

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

---

<div style="display: flex; justify-content: space-between; align-items: center; padding: 50px 0;">
    <a href="Section_2.md" style="padding: 5px 10px; background-color: #007bff; color: white; text-decoration: none; margin-right: auto; border-radius: 5px;">Previous</a>
    <span style="flex-grow: 1;"></span>
    <a>              </a>
    <a href="Section_4.md" style="padding: 5px 10px; background-color: #007bff; color: white; text-decoration: none; border-radius: 5px;">Next</a>
</div>

---