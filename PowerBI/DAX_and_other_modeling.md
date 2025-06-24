# <img src="../books.svg" alt="Stack of red books with a graduation cap on top, symbolizing education and achievement, set against a plain background" width="30" height="20" /> PL-300 Certification Prep: Microsoft Power BI Data Analyst

## <img src="../notes.svg" alt="Orange pencil lying diagonally on a white sheet of paper, representing note taking and documentation, with a clean and organized appearance" width="20" height="15" /> Other Modeling and DAX

### Role-Playing Dimensions

Is a dimension (table) that can slice—or filter—on another table in more than one way. They can take on many different roles! They are dimensions that are used multiple times or with multiple relationships with the same table.

- Dotted line means you have the "make relationship active" unchecked
  - In DAX, you can only have one link between a pair of tables
  - ***Role-playing models*** happen where there is more than one relationship where they can't both be active
  - To fix:
    - Way 1
      - Add new column with `USERELATIONSHIP()`, which allows you to use a different relationship. You can use `CALCULATE()` to create a new filter
      - Then you can create a new visual with the new column
    - Way 2
      - Create a separate table!
      - i.e. DateTable2 = DateTable
      - PowerBI can create copies

### Many-To-Many Relationships

- Examples:
  - Joint bank accounts
- The "make this relationship active" box must be checked in order for the relationship to apply
  - The cross filter direction should be both ways unless your data only goes in one direction
- Note: you can't use `RELATED()` on either side, because it won't bring back a single row, it may bring back multiple rows

### Different Types of Granularity

If you have data that exists in one table, but doesn't exist in the other, you can create a third table called a ***bridging table*** that contains the common factor.

- To create a bridging table:
  1. Append the two tables using an APPEND query
  2. De-duplicate to remove duplicated information
  3. Give this table the active relationship
  4. Hide the columns from the two tables you used to create the bridging table to make the experience easier on the user (otherwise, you will see 3 country columns!)

### Improving Cardinality Levels Through Summarization and by Changing Data Types

- Two ways to create ***summary tables***:
  1. `GROUPBY()` in the edit query - reduces the table downwards
  2. Create a new summary table using `SUMMARIZECOLUMNS()`

#### Levels of Cardinality

- High cardinality
  - No or minimal duplication, highly specified
    - No duplication is the highest cardinality
  - One unique row per value
  - e.g. Primary Keys
- Normal cardinality
  - e.g Names
- Low cardinality
  - Many rows for each value
  - Limited number of values
  - e.g True/False

### Identify Poorly Performing Measures, Relationships, and Visuals

#### Performance Analyzer Pane

Assesses your report's performance and areas of improvement

Steps:

1. Create a blank page
2. Performance Analyzer
3. Start recording
4. Go to the page with your visualization
5. Expand the visualization
    - *Visual display* - time to take to render the visual on the screen
      - Every visual has a display cost!
    - *DAX query* - a request to get to the tabula engine
      - If you copy this query and paste it in your notebook, you will see the query that is sent
    - *Other* - time spent waiting, bottlenecks, etc
      - May be something on your specific computer, network, SQL server database, and may not be helpful. Try refreshing!
      - Google some key words in combination with each other to see if there are better, quicker ways to do what you are trying to achieve

### DAX Query View

Allows you to run DAX queries. The advantage of this is it allows you to *modify them individually* without having to export them to the model. ***You can change the definition of a measure and see how it performs against the different version without having to import it.*** Accessed via the *fourth* icon on the left hand side or by clicking "run in DAX query view from the performance analyzer.

`EVALUATE()` is `SELECT()` or `print()` in other languages

Defining all measures in the table using `DEFINE()` will include the `MEASURE()` query, which defines variables to measure and the formulas that make them.

#### Other DAX Queries

- `NATURALINNERJOIN()` - Includes all the columns in both queries where there is a match.
- `NATURALLEFTOUTERJOIN()` - Includes all of the rows in the first table (or left table) regardless whether there is a match or not


## <img src="../question-and-answer.svg" alt="Two speech bubbles, one with a large letter Q and the other with a large letter A, representing a question and answer exchange in a friendly and approachable style" width="35" height="28" /> Cues

- What DAX function combines one query with the columns of another query?
- What is a role-playing dimension?
- When you use the Performance Analyzer pane to identify poorly performing measures and visuals, what is the next step after you open the analyzer?

---

## <img src="../summary.svg" alt="Rolled parchment scroll with visible lines, symbolizing a summary or conclusion, placed on a neutral background" width="30" height="18" /> Summary

xxx
