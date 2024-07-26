<details>
  <summary>Table of Contents</summary>
  <ul>
    <li><a href="/README.md">Home</a></li>
    <li><a href="../Chapter 1/Chapter_1_Home.md">Chapter 1</a></li>
    <li><a href="Chapter_2_Home.md">Chapter 2</a></li>
    <li><a href="../Chapter 3/Chapter_3_Home.md">Chapter 3</a></li>
    <li><a href="../Chapter 4/Chapter_4_Home.md">Chapter 4</a></li>
    <li><a href="../Chapter 5/Chapter_5_Home.md">Chapter 5</a></li>
    <li><a href="../Chapter 6/Chapter_6_Home.md">Chapter 6</a></li>
  </ul>
</details>

# Chapter 2: Testing Throughout the Software Development Lifecycle

## Description

- It is estimated that you should take around 130 minutes (2 Hours and 10 minutes) to learn.
- In this chapter learn:

  - How testing is incorporated into different development approaches
  - Concepts of test-first approaches, as well as DevOps
  - Different test levels
  - Different test types
  - Different Maintenance testing

- Knowledge Levels
  - K1: Remember - You should remember/recognize a term or a concept
  - K2: Understand - You should be able to select an explanation for a statement related to the question topic

## Learning Objectives for Chapter 2

- [Testing in the Context of a Software Development Lifecycle](#21)
  - [(K2) Explain the impact of the chosen SDLC on testing](#211)
  - [(K1) Recall good testing practices that apply to all SDLC](#212)
  - [(K1) Recall the examples of Test-First approaches to development](#213)
  - [(K2) Summarize how DevOps might have an impact on testing](#214)
  - [(K2) Explain the Shift-Left Approach](#215)
  - [(K2) Explain how retrospectives can be used as a mechanism for process improvement](#216)
- [Test Levels and Test Types](#22)
  - [(K2) Distinguish the different test levels](#221)
  - [(K2) Distinguish the different test types](#222)
  - [(K2) Distinguish confirmation testing from regression testing](#223)
- [Maintenance Testing](#23)
  - [(K2) Summarize maintenance testing and its triggers](#231)

<a id="21"></a>

## (2.1) Testing in the Context of SDLC

- **SDLC Models:**
  - Sequential Development Models
    - Waterfall Model
    - V-Model
  - Iterative Development Models
    - Spiral Model
    - Prototyping
    - Agile
  - Incremental Development Models
    - Unified Process
- Software Development Methods and Agile Practices:

  - Acceptance Test-Driven Development (ATDD)
  - Behavior-Driven Development (BDD)
  - Domain-Driven Development (DDD)
  - Extreme Programming (XP)
  - Feature-Driven Development (FDD)
  - Test-Driven Development (TDD)
  - Kanban
  - Lean IT
  - Scrum

  <a id="211"></a>

  ## (2.1.1) Impact of the SDLC on Testing

  - SDLC choice impacts:

    - Scope and Timing of Test Activities
      - Test Levels
      - Test Types
    - Level of detail of Test Documentation
    - Choice of Test Techniques and Test Approach
    - Extent of Test Automation
    - Role and Responsibilities of a Tester

  - With **Sequential Development Models**:

    - Initial Phase Testers participate in:
      - Requirement Reviews
      - Test Analysis
      - Test Design
    - Later Phases:
      - Executable Code is created
    - Dynamic Testing usually cannot be performed early in SDLC

  - With **Iterative** and **Incremental Development Models**:
    - During each iteration:
      - Deliver a working prototype or product increment
      - Static and Dynamic Testing are performed at all test levels
      - Frequent delivery of increments require fast feedback and extensive Regression Testing

  Within **Agile**:
