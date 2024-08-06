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
- [(K3) Prepare a defect report](Section_5.md)

<a id=55></a>

## Defect Management
- A major test objective is to find defects, therefore established Defect Management Process is essential
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
  - Description of the failure to enable reproduction and resolution including the steps that detected the anomaly, and any relevant \_\_\_\_:
    - Test logs
    - Database Dumps
    - Screenshots
    - Recordings
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

- Some of the listed data may automatically included when using the defect management tools
  - Identifier
  - Date
  - Author
  - Initial Status

- Document templates for a defect report and example defect reports can be found in ISO/IEC/IEEE 29119-3 Standard