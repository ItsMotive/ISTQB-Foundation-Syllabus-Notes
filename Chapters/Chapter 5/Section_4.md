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
- [(K2) Summarize how configuration management supports testing](Section_4.md)

<a id=54></a>

## Configuration Management
- Provides discipline for \_\_\_\_ :
  - Identifying
  - Controlling
  - Tracking
- For work products such as \_\_\_\_ as configuration items:
  - Test Plans
  - Test Strategies
  - Test Conditions
  - Test Cases
  - Test Scripts
  - Test Results
  - Test Logs
  - Test Reports

- For a complex configuration item (Test Environment), CM records:
  - Items it consists of
  - Their Relationship
  - Versions

- If Configuration item is approved for testing, it becomes a baseline and can only be changed through a formal change control process

- Keeps a record of changed configuration items when a new baseline is created

- It is possible to revert to a previous baseline to reproduce previous test results

- To properly support testing, CM ensures the following:
  - All configuration items, including test items (individual parts of the test object), are \_\_\_\_ so that traceability can be maintained:
    - Uniquely identified
    - Version Controlled
    - Tracked for Changes
    - Related to other configuration items
  - All identified documentation and software items are referenced unambiguously in test documentation

- Automated CM is normally included in \_\_\_\_, typically implemented as part of an Automated [DevOps pipeline](/Chapters/Chapter%202/Section_1.md#214):
  - Continuous Integration
  - Continuous Delivery
  - Continuous Deployment
  - Associated Testing 