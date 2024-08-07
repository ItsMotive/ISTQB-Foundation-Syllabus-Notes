# Topics from Fundamentals of Testing Mock Test

## Description
Based on: https://istqb.patshala.com/tests/mode.php?tn=21 <br />
 
ISTQB topic based mock test: Static Testing Techniques

# Topics to Review
- [Walkthrough](#1)
- [Static Analysis Tool](#2)
- [Static Analysis](#3)
- [Inspections](#4)
- [Formal Review](#5)
- [Static Testing](#6)
- [Checklist](#7)
- [Review Process](#8)

<a id=1></a>

## Walkthrough
- Key Characteristics
    - Scenario
    - Dry Run
    - Peer Group

<a id=2></a>

## Static Analysis Tool
- Used by Developers
- Typical defects found:
    - Variables that are never used
    - Security vulnerabilities
    - Unreachable code

- Typical defects **NOT** found:
    - Poor performance
    - Business processes not followed

- **DOES**:
    - Gives quality information about the code without executing it

- **DOES NOT**:
    - Check expected results against actual results
    - Detect memory leaks
    - Give info about what code has and has not been exercised

<a id=3></a>

## Static Analysis
- **CAN** find:
    - Use of a variable before it has been defined
    - Unreachable ("dead") code
    - Undeclared variables
    - Array bound violations
    - Too few comments
    - Programming standard violations
    - Security vulnerabilities

- **CANNOT** find:
    - Memory leaks
    - Faults in the requirements
    - Whether the value stored in a variable is correct

<a id=4></a>

## Inspections
- Most formal review process
- Should be led by trained leader
- Managers can perform on management documents
- Compares documents with predecessor (source) documents
- **CANNOT** be done when there are no written documents

<a id=5></a>

## Formal Review
- Main Phases:
    - **Planning**
    - **Kick off**
    - **Individual Preparation**
    - **Review Meeting**
    - **Rework**
    - **Follow up**

- Typical defects easier to find
    - Deviations from standards
    - Requirement Defects
    - Design Defects

<a id=6></a>

## Static Testing
- Used in phases:
    - Requirements
    - Design
    - Coding

- Includes:
    - Desk Checking
    - Techniques such as reviews and inspections
    - Giving measurements such as cyclomatic complexity
    - **NOT** running tests through the code

<a id=7></a>

## Checklist
- Series of probing questions about the completeness and attributes of an application system

<a id=8></a>

## Review Process
- Inspection
    - Persons involved:
        - Led by a trained moderator or leader
        - Managers can perform on management documents
        - Scribe/Recorder
    - Uses Entry/Exit Criteria
    - Most formal review process
    - Compares documents with predecessor (source) documents
    - **CANNOT** be done when there are no written documents

- Peer Review
    - No management participation

- Informal Review
    - Undocumented

- Walkthrough
    - Led by Author
