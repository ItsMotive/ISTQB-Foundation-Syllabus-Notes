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
- [(K2) Explain how to write user stories in collaboration with developers and business representatives](#451)
- [(K2) Classify the different options for writing acceptance criteria](#452)
- [(K3) Use acceptance test-driven development (ATDD) to derive test cases](#453)

<a id=45></a>

## (4.5) Collaboration-Based Test Approaches
- Sections [4.1](Section_1.md), [4.3](Section_3.md), [4.4](Section_4.md) techniques have a particular objective with respect to defect detection
- On the other hand Collaboration-Based approaches also focus on defect avoidance by collaboration and communication

  <a id=451></a>

  ## (4.5.1) Collaborative User Story Writing
  - **User Story**
    - Represents a feature that will be valuable to either a user or purchaser of a system or software
    - Three critical aspects:
      - **Card** - Medium describing a user story
        - Index Card
        - Entry in an electronic board

      - **Conversation** - Explains how the software will be used
        - Verbally
        - Documented

      - **Confirmation**
        - The [Acceptance Criteria](#452)
      
  - Common Format:
    - As a [role] 
    - I want [goal to be accomplished]
    - so that I can [resulting business value for the role]
    - Followed by the Acceptance Criteria
  
  - Collaborative Authorship of the user story can use techniques:
    - Brainstorming
    - Mind Mapping

  - Collaboration allows team to obtain shared vision of what should be delivered by taking into account three perspectives:
    - Business
    - Development
    - Testing

  - Good user stories should be (INVEST):
    - Independent 
    - Negotiable
    - Valuable
    - Estimable
    - Small 
    - Testable 
  
  - If stakeholder does not know how to test a user story, it may indicate:
    - User story is not clear enough
    - Does not reflect something valuable to them
    - Stakeholders just needs help in testing

  <a id=452></a>

  ## (4.5.2) Acceptance Criteria
  - Conditions that an implementation for the user story must meet to be accepted by stakeholders
  - May be viewed as the the test conditions that should be exercised by the tests
  - Result of the [Conversation](#451)

  - Acceptance Criteria are used to:
    - Define scope of the User Story
    - Reach consensus among stakeholders
    - Describe both positive and negative scenarios
    - Serve as a basis for the User Story [Acceptance Testing](#453)
    - Allow accurate planning and estimation

  - Several ways to write Acceptance Criteria for User Story
  - 2 Common formats:
    - Scenario-Oriented:
      - Given/When/Then Format used in [BDD](/Chapters/Chapter%202/Section_1.md#213)
    - Rule-Oriented:
      - Bullet point verification list
      - Tabulated form of Input-Output Mapping

  <a id=453></a>
  ## (4.5.3) Acceptance Test-Driven Development (ATDD)
  - A [Test-First Approach](/Chapters/Chapter%202/Section_1.md#213)
  - Test cases are created:
    - Prior to implementing the user story
    - By team members with different perspectives
      - Customers
      - Developers
      - Testers

  - Acceptance Criteria
    - May detail some issues described in the user story

  - Test cases 
    - Can be manual or automated
    - Should be expressed in a way that is understandable for the stakeholders
    - Contain sentences in natural language involving the necessary:
      - Preconditions
      - Inputs
      - Postconditions
    - Must cover all characteristics of the user story
    - Not go beyond the story
    - No two should describe the same characteristics of the user story

  - **First Step**
    - Specification workshop where the user story and (if not defined yet) its acceptance criteria are \_\_\_\_ by team members:
      - Analyzed
      - Discussed
      - Written

    - During this process, it can resolve \_\_\_\_ in the user story:
      - Incompleteness
      - Ambiguities
      - Defects

  - **Next Step**
    - Create Test Cases
      - Whole Team
      - Tester individually
    - Test Cases are:
      - Based on Acceptance Criteria
      - Seen as examples of how software works
      - Helpful for the team to implement user stories correctly

  - These terms are interchangeable:
    - Tests
    - Examples
  
  - First test cases are positive: 
    - Confirming correct behavior without exceptions or error conditions
    - Comprising the sequence of activities executed if everything goes as expected
  
  - After positive tests, negative testing should be performed
  - Finally, team should cover non-functional quality characteristics as well
    - Performance Efficiency
    - Usability

  - Acceptance Tests can become executable requirements
    - Captured in a format supported by test automation framework
    - Developers can automate the test cases by writing supporting code as they implement the feature described by user story