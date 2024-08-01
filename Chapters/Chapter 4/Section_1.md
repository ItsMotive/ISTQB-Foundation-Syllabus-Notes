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
- [(K2) Distinguish black-box, white-box and experience-based test techniques](#41)

<a id=41></a>

## (4.1) Test Techniques Overview
- Supports tester in Test Analysis (what to test) and Test Design (how to test)
- Helps to develop relatively small, but sufficient, set of test cases in a Systematic way
- Helps tester _\_\_\_ during Test Analysis and Design:
    - Define Test Conditions
    - Identify coverage items
    - Identify Test Data

- **Black-Box Test Technique**
    - Referred to as Specification-Based Techniques
    - Based on analysis of the specified behavior of the test object without code knowledge
    - Test cases are independent on how software is implemented
        - If there are code changes, but required behavior stays the same, test cases will stay useful

- **White-Box Test Techniques**
    - Referred to as Structure-Based Techniques
    - Based on analysis of the test object's internal structure and processing
    - Test cases are dependent on how the software is designed
        - Created only after design or implementation of the test object

- **Experience-Based Test Techniques**
    - Makes use of knowledge and experience of testers for the design and implementation test cases
    - Effectiveness depends on tester's skills
    - Complementary to other techniques due to the ability of finding defects not found in the others