# Read 14a - dB Normalization

#### 2020-03-26

## RESOURCES:
#### Database Normalization Explained in Simple English <br>
https://www.essentialsql.com/get-ready-to-learn-sql-database-normalization-explained-in-simple-english/ <br>

### Database normalization <br>
__Database normalization__ is a process used to organize a database into tables and columns.  The main idea with this is that a table should be about a specific topic and only supporting topics included. __*By limiting a table to one purpose*__ you reduce the number of duplicate data contained within your database. This eliminates some issues stemming from database modifications. <br>

__*There are three normal forms most databases adhere to using*__.  As tables satisfy each successive database normalization form, they become less prone to database modification anomalies and more focused toward a sole purpose or topic. <br>

When a table has more than one purpose, maintaining it becomes difficult.  Some of the problems doing so are categorized as follows: <br>
#### Insert Anomaly <br>
There are facts we cannot record until we know information for the entire row. <br>
#### Update Anomaly <br>
Happens when have the same information in several rows. If we don’t update all rows, then inconsistencies appear. <br>
#### Deletion Anomaly <br>
Deletion of a row causes removal of more than one set of facts. <br>

Not having a normalized database can also lead to Search and Sort Issues. <br>

There are three common forms of database normalization: __1st, 2nd, and 3rd normal form__. They are also abbreviated as __1NF, 2NF,__ and __3NF__ respectively. __*The forms are progressive*__, meaning that to qualify for 3rd normal form a table must first satisfy the rules for 2nd normal form, and 2nd normal form must adhere to those for 1st normal form. Before we discuss the various forms and rules in detail, let’s summarize the various forms: <br>

### First Normal Form <br>
__*"The information is stored in a relational table with each column containing atomic values."*__ There are no repeating groups of columns. When a value is atomic, the values cannot be further subdivided. <br>

### Second Normal Form <br>
__*"The table is in first normal form and all the columns depend on the table’s primary key."*__ We place tables in 2nd normal form is to narrow them to a single purpose. This stems from the primary key identifying the main topic at hand, such as identifying buildings, employees, or classes, and the columns, serving to add meaning through descriptive attributes. When all the columns relate to the primary key, they naturally share a common purpose. <br>

### Third Normal Form <br>
__*"The table is in second normal form and all of its columns are not transitively dependent on the primary key."*__ When something is transitive, then a meaning or relationship is the same in the middle as it is across the whole. In general, if A is greater than B, and B is greater than C, then it follows that A is greater than C. __*'Transitive dependence'*__ means a column’s value relies upon another column through a second intermediate column. <br>

"Can database normalization be taken too far?  You bet!  There are times when it isn’t worth the time and effort to fully normalize a database." <br>
