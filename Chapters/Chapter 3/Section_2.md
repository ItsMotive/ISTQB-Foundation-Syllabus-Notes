<details>
  <summary>Table of Contents</summary>
  <ul>
    <li><a href="/README.md">Home</a></li>
    <li><a href="Chapter_3_Home.md">Chapter Home</a></li>
    <li><a href="Section_1.md">Section 1</a></li>
    <li><a href="Section_2.md">Section 2</a></li>
  </ul>
</details>

# Section Guide

- [(K1) Identify the benefits of early and frequent stakeholder feedback](#321)
- [(K2) Summarize the activities of the review process](#322)
- [(K1) Recall which responsibilities are assigned to the principal roles when performing reviews](#323)
- [(K2) Compare and contrast the different review types](#324)
- [(K1) Recall the factors that contribute to a successful review](#325)

<a id=32></a>

## (3.2) Feedback and Review Process
- Going over Feedback and Review Process

    <a id=321></a>

    ## (3.2.1) Benefits of Early and Frequent Stakeholder Feedback
    - Early communication of potential quality problems
    - Project development more likely to meet stakeholder's original or current vision with more stakeholder involvement during SDLC
    - Failure to deliver stakeholder's vision results in:
        - Costly rework
        - Missing deadlines
        - Blame games
        - Complete project failure
    - Prevents requirement misunderstandings
    - Ensures changes to requirements are understood and implemented earlier
    - Development team has a better understanding of what they're building
    - Focus on features that deliver the most value to the stakeholders 
    - Focus on features that have the most positive impact on identified risks

    <a id=322></a>

    ## (3.2.2) Review Process Activities
    - Review process may be done multiple times in order for completion due to size of work products
    - Activities:
      - **Planning**
        - Scope of the review is defined
          - Purpose
          - Work Product to be reviewed
          - Quality characteristics to be evaluated
          - Areas to focus on
          - Exit Criteria
          - Supporting information such as standards
          - Effort
          - Time frames for the review

      - **Review Initiation**
        - Goal:
          - Everyone and everything involved is prepared to start the review
          - Every participant has access to the work product under review
          - Every participant understands their role and responsibilities and receives everything needed for review

      - **Individual Review**
        - Each reviewer performs an individual review to assess the quality of work product under review
          - This helps to identify:
            - Anomalies
            - Recommendations
            - Questions
          - Uses Review Techniques:
            - Checklist-Based Reviewing
            - Scenario-Based Reviewing
        - Reviewers logs everything identified

      - **Communication and Analysis**
        - Anomalies found aren't all defects, so they will need to be analyzed and discussed
        - Each anomaly needs a decision on:
          - Status
          - Ownership
          - Required Actions
        - The decisions are usually made in Review Meetings
          - Participants decide quality level of the reviewed product and if follow-up actions are required
        - Follow-up review may be required to complete actions

      - **Fixing and Reporting**
        - Every defect requires a defect report so that corrective actions can be followed up
        - Once Exit criteria is reached, work product can be accepted
        - Review results are reported

    <a id=323></a>

    ## (3.2.3) Roles and Responsibilities in Reviews
    - Various stakeholders may take on several roles
    - More roles can be found in ISO/IEC 20246 Standard
    - Principle roles and their responsibilities:

      - **Manager** 
        - Decides what is to be reviewed and provides resources
          - Staff
          - Time for the review

      - **Author**
        - Creates and fixes the work product under review

      - **Moderator (Facilitator)**
        - Ensures effective running of review meetings
          - Mediation
          - Time Management
          - Safe Review environment
            - So everyone can talk freely
      
      - **Scribe (Recorder)**
        - Collect and combine anomalies from reviewers
        - Records review information
          - Decisions
          - New anomalies found during the review meeting
      
      - **Reviewer**
        - Performs Reviews
        - Can be:
          - Someone working on the project
          - Subject Matter Expert (SME)
          - Any other stakeholder

    <a id=324></a>

    ## (3.2.4) Review Types
    - Informal and Formal Reviews
    - Formality level is dependent on:
      - SDLC being followed
      - Maturity of development process
      - Criticality and Complexity of Work Product being reviewed
      - Legal and regulatory requirements
      - Need for an audit trail
    - Same Work Product can be reviewed with different types:
      - First an Informal
      - Then a Formal
    - Selecting the right review type is key to achieving the required [Review Objective](#325).
    - Selection is based on:
      - Objectives
      - Project needs
      - Available resources
      - Work Product types and risks
      - Business domain
      - Company culture
    - Commonly used Review Types:
      - **Informal Review**
        - Does not follow a defined process
        - Does not require a formal document output
        - Main Objective:
          - Detecting anomalies

      - **Walkthrough**
        - Led by Author
        - Serve many objectives:
           - Evaluating quality
           - Building confidence in:
            - Work Product
            - Educating Reviewers
            - Gaining consensus
            - Generating new Ideas
            - Motivating
            - Enabling Authors to improve and detect anomalies
        - Reviewers might perform an individual review before walkthrough, but is not required

      - **Technical Review**
        - Led by Moderator
        - Performed by technically qualified reviewers
        - Objective:
          - Gain census 
          - Make decisions regarding a technical problem
          - Detect anomalies
          - Evaluate quality
          - Build confidence in Work Product
          - Generate new ideas
          - Motivate and enable Authors to improve

      - **Inspection**
        - Most formal type of review
        - Follows a complete [generic process](#322)
        - Main Objective:
          - Find maximum number of anomalies
        - Other Objectives
          - Evaluate quality
          - Build Confidence in the Work product
          - Motivate and enable Authors to Improve
        - Metrics are collected and used to improve the SDLC
        - Author cannot act as the Review Leader or Scribe

    <a id=325></a>

    ## (3.2.5) Success Factors for Reviews
    - Defining clear objectives and measurable exit criteria
      - Evaluation of participants should never be an objective
    - Choosing the appropriate review type to achieve the given objectives and to suit:
      - Type of work product
      - Review participants 
      - Project needs and context
    - Conducting reviews on small chunks
      - Ensures reviewers do not lose concentration during an individual review and/or the review meeting (when held)
    - Providing feedback from reviews to Stakeholders and Authors
      - Allows them to improve the product and their [activities](#321)
    - Provides adequate time for participants to prepare for the review
    - Support from management for the review process
    - Making reviews part of the organization's culture
      - Promotes learning and process improvement
    - Providing adequate training for all participants
      - Allows them to know how to fulfill their role
    - Facilitate meetings