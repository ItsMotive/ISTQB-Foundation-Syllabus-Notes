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
- [(K3) Use equivalence partitioning to derive test cases](#421)
- [(K3) Use boundary value analysis to derive test cases](#422)
- [(K3) Use decision table testing to derive test cases](#423)
- [(K3) Use state transition testing to derive test cases](#424)

<a id=42></a>

## Black-Box Test Techniques
- Commonly used techniques:
    - Equivalence Partitioning
    - Boundary Value Analysis
    - Decision Table Testing
    - State Transition Testing

    <a id=421></a>

    ## Equivalence Partitioning
    - Divides data into partitions
    - Partitions can be:
        - Continuous or discrete
        - Ordered or unordered
        - Finite or infinite
    - Theory:
        - If a test case tests one value from a partition and detects a defect
        - Then this defect should also be detected with other values within the same partition
        - Therefore one test for each partition is sufficient
    - Can be identified for any data element related to test object:
        - Inputs
        - Outputs
        - Configuration items
        - Internal values
        - Time-Related values
        - Interface parameters
    - Simple test objects EP <u>CAN</u> be easy
        - In practice though, understanding how the test object wil treat different values is often complicated
        - **Partitioning SHOULD BE done with care**
    - **Valid Partition**
        - Partition containing valid values
            - Example - Valid values may be interpreted as those that should be processed by the test object or as those for which the specification defines their processing
    - **Invalid Partition**
        - Partition containing invalid values
            - Example - Invalid values may be interpreted as those that should be ignored or rejected by the test object or as those for which no processing is defined in the test object specification
    - Definition of valid and invalid values dependent on team and organization
    - Coverage items are the Equivalence Partitions
    - Achieving 100% Coverage:
        - Test cases must exercise all identified partitions (includes invalid partitions) by covering each partition at least once
    - Coverage is measured by:
        - Number of partitions exercised by at least one test case
        - Divided by the total number of identified partitions
        - Coverage is expressed as a percentage
    - Many test objects include multiple sets of partitions
        - Test objects with more than one input parameter
        - Which means a test case will cover partitions from different sets of partitions
    - Each Choice Coverage
        - Simplest coverage criterion in the case of multiple sets of partitions
        - Each choice coverage requires test cases to exercise each partition from each set of partitions at least once
        - Each one does not take into account combinations of partitions

    <a id=422></a>

    ## Boundary Value Analysis
    - Based on exercising the boundaries of Equivalence Partitions
        - Can only be used for ordered partitions
        - This is due to developers more likely to make errors with these boundary values

    - Minimum and Maximum values of a partitions are its boundary values
    - If two elements belong to the same partition, all elements between them must also belong to that partition

    - Two Versions of BVA:
        - **2-Value BVA**
            - For each boundary value, there should be 2 coverage items:
                - The boundary value 
                - Closest neighbor belonging to adjacent partition
            - Achieving 100% coverage:
                - Test cases must exercise all coverage items
                    - All Identified boundary values
            - Coverage is measured as:
                - Number of boundary values exercised
                - Divided by total number of identified boundary values
                - Expressed as a percentage

        - **3-Value BVA**
            - For each boundary value, there should be 3 coverage items:
                - The boundary value
                - Both neighbors belonging to adjacent partition
            - Coverage items may not be boundary values
            - Achieving 100% coverage:
                - Test cases must exercise all coverage items:
                    - Identified boundary values
                    - Their neighbors
            - Coverage is measured as:
                - Number of boundary values and their neighbors exercised
                - Divided by the total number of identified boundary values and their neighbors
                - Expressed as a percentage
            - More vigorous than 2-Value BVA, due to being able to detect defects overlooked
            - Example:
                - Decision "if (x <= 10)"
                - Incorrectly implemented as "if (x = 10)"
                - 2-Value BVA (x = 10, x = 11), no test data derived can detect the defect
                - 3-Value BVA (x = 9, x = 10, x = 11) is likely to detect the defect

    <a id=423></a>

    ## Decision Table Testing
    - Used for testing implementation of system requirements that specify how different combinations of conditions result in different outcomes
    - Effective way of recording complex logic, such as business rules
    - Table Rows
        - Conditions and resulting actions of the system are defined

    - Table Columns
        - Corresponds to a decision rule that defines a unique combination of conditions
        - Along with associated actions

    - **Limited-Entry Decision Table**
        - All values of the conditions and actions (except for irrelevant or infeasible ones) are shown as Boolean values (True or False)

    - **Extended-Entry Decision Table**
        - Some or all conditions or actions may take on multiple values
            - Ranges of numbers
            - Equivalence partitions
            - Discrete Values

    - Notation for Conditions:
        - **"T"** : True - Condition satisfied
        - **"F"** : False - Condition is not satisfied
        - **"-"** : Value of condition is irrelevant for action outcome
        - **"N/A"** : Condition is infeasible for a given rule

    - Notation for Actions:
        - **"X"** : Action should occur
        - **"Blank"** : Action should not occur
        - Other notations may be used

    - Full decision table has enough columns to cover every combination of conditions
    - Table can be simplified by: 
        - Deleting columns containing infeasible combinations of conditions
        - Merging columns where conditions do not affect the outcome into a single column
        - Minimization algorithms are out of scope of syllabus
    - Coverage items are the columns containing feasible combinations of conditions
    - Achieving 100% Coverage:
        - Test cases must exercise all these columns
        - Number of exercised columns
        - Divided by total number of feasible columns
        - Expressed as a percentage
    - Provides systematic approach to identify all combinations of conditions where some might be overlooked
    - Helps find any gaps or contradictions in the requirements
    - If there are many conditions:
        - Exercising all the decision rules may be time consuming
            - Number of rules grows exponentially with the number of conditions
        - Reduce the number of rules that need to be exercised
        - Minimized decision table
        - Risk-Based approach

    <a id=424></a>
    
    ## State Transition Testing
    - **State Transition Diagram** 
        - Models the behavior of a system by showing its possible states and valid state transitions
        - Transition is initiated by an event
            - May be additionally qualified by a guard condition
        - Transitions are assumed to be instantaneous and may sometimes result in the software taking action
        - Common Transition Labeling:
            - "Event [guard condition] / Action"
        - Guard conditions and actions can be omitted if they do not exist or are irrelevant for the tester
    
    - **Stable Table**
        - Equivalent Model to State Transition Diagram
        - **Rows** represent states
        - **Columns** represent events (together with guard conditions if they exist)
        - **Table Entries (Cells)** represent transitions and contains:
            - Target State
            - Resulting Actions, if defined
        - In contrast to Transition Diagram, State Table explicitly shows invalid transitions
            - Represented by empty cells

    - Test case based on a State Transition Diagram or Stable Table is usually represented as a sequence of events
        - Results in a sequence of state changes (and actions if necessary)
    - One test case may, and usually will, cover several transitions between states
    - There exists many coverage criteria for state transition testing

    - **All States Coverage**
        - Coverage items are the states
        - Achieving 100% Coverage:
            - Test cases must ensure all states are visited
            - Number of visited states
            - Divided by the total number of states
            - Expressed as a percentage

    - **Valid Transitions Coverage**
        - Also called 0-Switch Coverage
        - Coverage items are single valid transitions
        - Achieving 100% Coverage:
            - Test cases must exercise all the valid transitions
            - Number of exercised valid transitions
            - Divided by the total number of valid transitions
            - Expressed as a percentage

    - **All Transitions Coverage**
        - Coverage items are all transitions show in a State Table
        - Testing only one invalid transition in a single test case helps to avoid fault masking
            - Situation in which one defect prevents the detection of another
        - Achieving 100% Coverage:
            - Test cases must exercise all the valid transitions and attempt to execute invalid transitions
            - Number of valid and invalid transitions exercised or attempted to be covered by executed test cases
            - Divided by the total number of valid and invalid transitions
            - Expressed as a percentage
    
    - **All States Coverage** is weaker than **Valid Transitions Coverage**
        - Due to it typically being able to achieve without exercising all the transitions
    - **Valid Transitions** is the most widely used coverage criterion
    - Achieving full **Valid Transition Coverage** guarantees full **All States Coverage**
    - Achieving full **All Transitions Coverage** guarantees both full **All States Coverage** and full **Valid Transitions Coverage**
        - Should be a minimum requirement for mission and safety-critical software