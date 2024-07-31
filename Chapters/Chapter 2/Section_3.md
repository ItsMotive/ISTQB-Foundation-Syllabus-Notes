<details>
  <summary>Table of Contents</summary>
  <ul>
    <li><a href="/README.md">Home</a></li>
    <li><a href="Chapter_2_Home.md">Home</a></li>
    <li><a href="Section_1.md">Section 1</a></li>
    <li><a href="Section_2.md">Section 2</a></li>
    <li><a href="Section_3.md">Section 3</
  </ul>
</details>

# Section Guide
  - [(K2) Summarize maintenance testing and its triggers](Section_3.md)

## (2.3) Maintenance Testing
- Different Categories:
  - Corrective
  - Adaptive to changes in the environment
  - Improve performance or maintainability
  
- Can involve:
  - Planned Releases/Deployments
  - Unplanned Releases/Deployments (Hot Fixes)

- Impact Analysis may be done before a change is made
  - Helps decide if change is necessary

- Production change testing includes evaluating successful implementation and checking possible regressions on unchanged parts of the system

- Scope depends on:
  - Degree of risk of the change
  - Size of the existing system
  - Size of the change
  
- Triggers for maintenance and maintenance testing can be classified as:
  - Modifications such as planned enhancements (Release-Based), corrective changes, or hot fixes
  - Upgrades or migrations of the operational environment
    - Can require tests associated with new environment, changes in software, or tests of data conversion
  - Retirement of a system
    - Testing of data archiving if long late-retention periods are required.
    - Testing of restore and retrieval procedures after archiving
  