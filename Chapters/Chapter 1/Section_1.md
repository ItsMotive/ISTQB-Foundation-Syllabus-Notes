<details>
  <summary>Table of Contents</summary>
  <ul>
    <li><a href="/Chapter_1_Home.md">Home</a></li>
    <li><a href="Section_1.md">Section 1</a></li>
    <li><a href="Section_2.md">Section 2</a></li>
    <li><a href="Section_3.md">Section 3</a></li>
    <li><a href="Section_4.md">Section 4</a></li>
    <li><a href="Section_5.md">Section 5</a></li>
  </ul>
</details>

<a id="11"></a>

## (1.1) What is Testing?

**Software Testing...**

- Assesses Software Quality and helps reducing the risk of software failure.
- Set of activities to find defects and evaluate the quality of software artifacts.
- May be [Static](Chapter%203.md) or [Dynamic](Chapter%204.md).
- Is technical and needs to be properly [Planned, Managed, Estimated, Monitored, and Controlled](Chapter%205.md).
- Is an intellectual activity, requiring testers to have specialized knowledge, use analytical skills, and apply critical thinking and systems thinking.
- Uses [Tools](Chapter%206.md)

  <a id="111"></a>

  ## (1.1.1) Test Objectives

  - **Typical Objectives:**

    - Evaluating work products such as requirements, user stories, designs, and code.
    - Triggering failures and finding defects.
    - Ensuring required coverage of a test object.
    - Reducing the level of risk of inadequate software quality.
    - Verifying whether specified requirements have been fulfilled.
    - Verifying that a test object complies with contractual, legal, and regulatory requirements.
    - Providing information to stakeholders to allow them to make informed decisions.
    - Building confidence in the quality of the test object.
    - Validating whether the test object is complete and works as expected by the stakeholders.

  - **Objectives are dependent on context:**
    - Work product being tested
    - Test Level
    - Risks
    - SDLC being followed
    - Factors related to the business context:
      - Corporate Structure
      - Competitive Considerations
      - Time to Market

  <a id="112"></a>

  ## (1.1.2) Testing and Debugging

  - **Testing:** Triggers failure that are caused by defects in the software or finds defects in the test object.

  - **Debugging:** Finds causes for defect/failure, analyzes, and eliminates them.

  - **Debugging Process:**

    - Reproduction of a failure
    - Diagnosis (Finding Root Cause)
    - Fixing the cause

  - **Subsequent Confirmation Testing** - Initial Tester checks whether the fixes resolved the problem.
  - **Subsequent Regression Testing** - Checks whether the fixes are causing failures in other parts of the test object. [(Section 2.2.3)](Chapter%202.md#223)
  - With Static Testing, there is no need for reproduction or diagnosis, since it directly finds defects and cannot cause failures.
