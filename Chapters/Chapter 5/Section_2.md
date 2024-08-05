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
- [(K1) Identify risk level by using risk likelihood and risk impact](#521)
- [(K2) Distinguish between project risks and product risks](#522)
- [(K2) Explain how product risk analysis may influence thoroughness and scope of testing](#523)
- [(K2) Explain what measures can be taken in response to analyzed product risks](#524)

<a id=52></a>

## (5.2) Risk Management
- There are many Internal and External factors that make it uncertain whether and when they will achieve their objectives (ISO 31000)
- Risk Management allows the organizations to increase the likelihood of:
  - Achieve objectives
  - Improve the quality of their products
  - Increase the stakeholders' confidence and trust

- Main Risk Management Activities:
  - Risk Analysis (Consists of [Risk Identification and Risk Assessment](#523))
  - Risk Control (Consists of [Risk Mitigation and Risk Monitoring](#524))

- Risk-Based Testing
  - Test Approach in which test activities are \_\_\_\_ based on Risk Analysis and Risk Control:
    - Selected
    - Prioritized
    - Managed

  <a id=521></a>
  
  ## (5.2.1) Risk Definition and Risk Attributes
  - Risk is a potential \_\_\_\_ whose occurrence causes an adverse effect:
    - Event
    - Hazard
    - Threat
    - Situation

  - Risk can be characterized by two factors:
    - Risk Likelihood
      - Probability of Risk Occurrence (greater than 0, less than 1)
    - Risk Impact (Harm)
      - Consequences of this occurrence
    - These factors express the risk level
      - Measure for the risk
      - Higher the risk level, the more important is its treatment
    
  <a id=522></a>

  ## (5.2.2) Project Risks and Product Risks
  - Software testing is generally concerned with 2 risks:
    - Project Risks
    - Product Risks

  - **Project Risks**:
    - Related to the management and control of the project
    - Includes:
      - Organizational Issues
        - Delays in work products deliveries
        - Inaccurate Estimates
        - Cost-Cutting

      - People Issues
        - Insufficient Skills
        - Conflicts
        - Communication Problems
        - Shortage of Staff

      - Technical Issues
        - Scope Creep
        - Poor Tool Support

      - Supplier Issues
        - Third-Party Delivery Failure
        - Bankruptcy of the supporting company
      
    - When they occur, they may impact project:
      - Schedule
      - Budget
      - Scope
    - This affects the project's ability to achieve its objectives

  - **Product Risks**
    - Related to the product quality characteristics
    - Examples:
      - Missing or Wrong Functionality
      - Incorrect Calculations
      - Runtime Errors
      - Poor Architecture
      - Inefficient Algorithms
      - Inadequate Response Time
      - Poor User Experience
      - Security Vulnerabilities

    - When they occur, they may result in various negative consequences:
      - User Dissatisfaction
      - Loss of Revenue, Trust, Reputation
      - Damage to third parties
      - High maintenance costs, overload of the helpdesk
      - Criminal Penalties
      - In Extreme Cases, physical damage, injuries, or death
    
  <a id=523></a>

  ## (5.2.3) Product Risk Analysis
  - From Testing Perspective:
    - Goal is to provide an awareness of Product Risk in order to focus the testing effort in a way to minimize the residual level of product risk
    - Ideally this occurs early in SDLC

  - Consists of:
    - **Risk Identification**
      - Generating a comprehensive list of risks
      - Stakeholders can identify risks by using various techniques and tools
        - Brainstorming
        - Workshops
        - Interviews
        - Cause-Effect Diagrams

    - **Risk Assessment**
      - Involves:
        - Categorization of identified risks
          - Helps in assigning mitigation actions
          - Risks in the same category can be mitigated using same approach
        - Determining their risk likelihood
        - Risk impact and level
        - Prioritizing
        - Proposing ways to handle the risks

      - Can use quantitative, qualitative, or mixed approach
        - Quantitative Approach
          - Risk level is calculated as the multiplication of risk likelihood and risk impact
        - Qualitative Approach
          - Risk level can be determined using a risk matrix

  - May influence the thoroughness and scope of testing
  - Results are used to:
    - Determine the scope of testing to be carried out
    - Determine the particular test levels and propose test types to be performed
    - Determine the test techniques to be employed and the coverage to be achieved
    - Estimate the test effort required for each task
    - Prioritize testing in an attempt to find the critical defects ASAP
    - Determine whether any activities in addition to testing could be employed to reduce risk

  <a id=524></a>

  ## Product Risk Control
  - Comprises all measures that are taken in response to identified and assessed product risks
  - Consists of Risk Mitigation and Risk Monitoring

    - **Risk Mitigation**
      - Involves implementing the actions proposed in Risk Assessment to reduce the risk level

    - **Risk Monitoring**
      - Ensure that the mitigation actions are effective, to obtain further information to improve risk assessment, and to identify emerging risks
  
  - With respect to Product Risk Control:
    - Once a risk has been analyzed, several response options to risk are possible:
      - Risk Mitigation by Testing
      - Risk Acceptance
      - Risk Transfer
      - Contingency Plan
  - Actions that can be taken to mitigate the product risks by testing:
    - Select testers with the right level of experience and skills, suitable for a given risk type
    - Apply an appropriate level of independence of testing
    - Conduct reviews and perform static analysis
    - Apply the appropriate test techniques and coverage levels
    - Apply the appropriate test types addressing the affected quality characteristics
    - Perform dynamic testing, including regression testing