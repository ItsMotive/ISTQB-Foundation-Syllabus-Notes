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
- [(K1) Recall metrics used for testing](#532)
- [(K2) Summarize the purposes, content, and audiences for test reports](#533)
- [(K2) Exemplify how to communicate the status of testing](#534)

<a id=53></a>

## (5.3) Test Monitoring, Test Control, and Test Completion
- **Test Monitoring**
  - Concerned with gathering information about testing
  - This information is used to:
    - Assess test progress 
    - Measure whether the test exit criteria or the test tasks associated with the exit criteria are satisfied
      - Meeting the targets for coverage of:
        - Product Risks
        - Requirements
        - Acceptance Criteria

- **Test Control**
  - Uses information from test monitoring to provide \_\_\_\_ to achieve the most effective and efficient testing:
    - Control Directives
    - Guidance
    - Necessary corrective actions
    - Examples:
      - Reprioritizing tests when an identified risk becomes an issue
      - Re-evaluating whether a test item meets entry criteria or exit criteria due to rework
      - Adjusting the test schedule to address a delay in the delivery of the test environment
      - Adding new resources when and where needed

- **Test Completion**
  - Collects data from completed test activities to consolidate:
    - Experience
    - Testware
    - Any other relevant information

  - Activities occur at project milestones:
    - Test level is completed
    - Agile Iteration is finished
    - Test project is completed (or cancelled)
    - Software system is released
    - Maintenance release is completed

  <a id=531></a>

  ## (5.3.1) Metrics used in Testing
  - Gathered to: 
    - Show progress against the planned schedule and budget
    - Current quality of the test object
    - Effectiveness of the test activities with respect to the objectives or an iteration goal
  - Test monitoring gathers a variety of metrics to support the test control and test completion
  - Common Test Metrics include:
    - Project progress metrics
      - Task Completion
      - Resource Usage
      - Test Effort
    - Test Progress Metrics
      - Test Case Implementation Progress
      - Test Environment Preparation Progress
      - Number of Test Cases run/not run
      - Number of Passed/Failed
      - Test Execution Time

  <a id=532></a>

  ## (5.3.2) Purpose, Content, and Audience for Test Reports
  - **Test Reporting** summarizes and Communicated test information during and after testing

  - **Test Progress Reports** support the ongoing control of the testing
    - When changes are needed due to deviation from the plan or changed circumstances, report must provide enough information to make modifications to:
      - Test Schedule
      - Resources
      - Test Plan

  - **Test Completion Reports** 
    - Summarize a specific stage if testing and can give information for subsequent testing
      - Test Level
      - Test Cycle
      - Iteration
    - Prepared during test completion, when a \_\_\_\_ is complete:
      - Project
      - Test level
      - Test type
    - Or ideally, the exit criteria have been met
    - Report uses test progress reports and other data
    - Typically includes:
      - Test Summary
      - Testing and Product quality evaluation based on the original test plan
        - Test Objectives
        - Exit Criteria
      - Deviations from the test plan
        - Differences from the planned schedule, duration, and effort
      - Testing impediments and workarounds
      - Test metrics based on test progress reports
      - Unmitigated risks, defects not fixed
      - Lessons learned that are relevant to the testing
  
  - During Test Monitoring and Control, test team generates test progress reports for stakeholder to keep them informed
  - Test Reports are usually generated on a regular basis and include:
    - Test Period
    - Test Progress including any notable deviations
      - Ahead or behind schedule
    - Impediments for testing and their workarounds
    - [Test Metrics](#531)
    - New and changed risks within testing period
    - Testing planned for the next period

  - Different audiences:
    - Require different information in the reports
    - Influence the degree of formality
    - The frequency of reporting
  
  - Test Progress Reporting to others in the same team is often frequent and informal
  - Project Testing Completion Reporting follows a set template and occurs only once

  - Test Completion Reports and Test Progress Reports (Test Status Reports) templates and examples can be found at ISO/IEC/IEEE 29119-3

  <a id=533></a>

  ## Communicating the Status of Testing
  - The best means of communicating test status varies, depending on:
    - Test management concerns
    - Organizational Test Strategies
    - Regulatory Standards
    - The team itself
      - In the case of [Self-Organizing Teams](/Chapters/Chapter%201/Section_5.md#152)
  - Options include:
    - Verbal Communication with team members and other stakeholders
    - Dashboards 
      - CI/CD Dashboards
      - Task Boards
      - Burn-Down Charts
    - Electronic Communication Channels
      - Email
      - Chat
    - Online Documentation
    - [Formal Test Reports](#532)
  
  - 1 or more options may be used
  - When face-to-face communication is not always possible, more formal methods may be more appropriate
  - Different stakeholders are interested in different types of information
    - Communication should be tailored accordingly