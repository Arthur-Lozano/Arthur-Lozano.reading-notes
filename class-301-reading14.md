# DB Normalization

> Database normalization is a process used to organize a database into tables and columns.  The main idea with this is that a table should be about a specific topic and only supporting topics included. Take a spreadsheet containing the information as an example, where the data contains salespeople and customers serving several purposes:

*  Identify salespeople in your organization
*  List all customers your company calls upon to sell a product
*  Identify which salespeople call on specific customers.

- Limiting a table to one purpose helps limit data redundancy by limiting the amount of duplicate data.

# Reasons for Database Normalization

* There are three main reasons to normalize a database.  

- The first is to minimize duplicate data

- The second is to minimize or avoid data modification issues

- The third is to simplify queries.

- Good to see tables that server one purpose

- Having the table serve many purposes introduces many of the challenges; namely, data duplication, data update issues, and increased effort to query data.

## Data Duplication and Modification Anomalies

*  Duplicated information presents two problems:

- It increases storage and decrease performance.

- It becomes more difficult to maintain data changes.

* These situations are modification anomalies. Database normalization fixes them. There are three modification anomalies that can occur:

- Insert Anomaly
> There are facts we cannot record until we know information for the entire row.  In our example we cannot record a new sales office until we also know the sales person.  Why?  Because in order to create the record, we need provide a primary key.  In our case this is the EmployeeID.

- Update Anomaly
> In this case we have the same information in several rows. For instance if the office number changes, then there are multiple updates that need to be made.  `If we don’t update all rows, then inconsistencies appear`.

- Deletion Anomaly
> Deletion of a row causes removal of more than one set of facts.  For instance, if John Hunt retires, then deleting that row cause us to lose information about the New York office.

### Search and Sort Issues

- The last reason we’ll consider is making it easier to search and sort your data.  In the SalesStaff table if you want to search for a specific customer such as Ford, you would have to write a query like

- One example would be looking for one property within a table.  We would have to look through each column to check if that property exists, instead we can create a seperate table that just holds those properties if it saves us time.

* The process to redesign the table is database normalization.

# Definition of Database Normalization

- There are three common forms of database normalization: 1st, 2nd, and 3rd normal form. They are also abbreviated as 1NF, 2NF, and 3NF respectively.
- There are various other forms such as BCNF.

### A summary of the forms

- First Normal Form – The information is stored in a relational table with each column containing atomic values. There are no repeating groups of columns.

- Second Normal Form – The table is in first normal form and all the columns depend on the table’s primary key.

- Third Normal Form – the table is in second normal form and all of its columns are not transitively dependent on the primary key.

- To progress to the next form the previous needs to be complete.

> For now it’s important to understand there are three rules for database normalization that upon each other.  Some people make database normalization seem complicated.




- Reference: ://www.essentialsql.com/get-ready-to-learn-sql-database-normalization-explained-in-simple-english/