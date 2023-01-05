# Pewlett-Hackard-Analysis

Database Keys
Database keys identify records from tables and establish relationships between tables. There are numerous types of keys. For our purposes, we will focus on primary keys and foreign keys.

Primary Keys
The departments.csv file has a dept_no column with unique identifiers for each row (one department number per department). For example, d001 will always reference the Marketing department, across other worksheets. This unique identifier is known as a primary key.

Primary keys are an important part of database design. When a database is being created, each table added must include a primary key in the architecture. Primary keys serve as a link between these tables.

Table 1( in deliverable 1) has a primary key, or column of unique identifiers in common with Tables 2 and 4. Table 3's primary key is linked only to Table 2. These links trace the relationships between tables. There are times when we'll need to trace two or three links to get the exact data we need. In these cases, we'll pick the data we need from each table. Linking the tables together in this manner is called a join, a feature we'll get into later.

In the second CSV file, dept_emp.csv, the "emp_no" column contains the primary key.

We know this is the primary key because each number is unique. For example, the emp_no column holds employee numbers. Each employee will have only one number, and that number won't be used for any other employee.


Foreign Keys
Foreign keys are just as important as primary keys. While primary keys contain unique identifiers for their dataset, a foreign key references another dataset's primary key.

Think about it like a phone number. You have your own number. It's your number, assigned to your phone, and unique to you. This is your primary key. Your friend also has a primary key: his or her own phone number.

When you save your friend's number in your phone, you're creating a reference to that person, also known as a foreign key. Your phone has lots of foreign keys (such as parents, doctors offices, friends, and other family), but only one primary key.

Likewise, when your friend saves your number in their phone, your number is now a foreign key in their phone. Saving these keys connects the devices. They show the relationship between your phone and your friend's phone.



In this example, dept_no shows up in both datasets; as an identifier (or primary key) in one and as a reference (or foreign key) in the other. This demonstrates the link between employees and which department they work in.

We could continue to look for connections between the datasets, or we could create a roadmap of the content. Our roadmap would serve as a quick reference diagramming the different datasets and their interconnections. Additionally, it could be used as a reference guide later, when we begin to create queries to access all of the data.

Table Structure
When working in Excel and Visual Basic for Applications (VBA), we're working directly with worksheets with data. In SQL, the same worksheets we have been exploring are organized into tables instead. They are similar to DataFrames in that they have headers and indexes, with data in columns and rows.



Entity Relationship Diagrams (ERDs)
An entity relationship diagram (ERD) is a type of flowchart that highlights different tables and their relationships to each other. The ERD does not include any actual data, but it does capture the following pertinent information from each CSV file:

Primary keys
Foreign keys
Data types for each column




Conceptual Diagrams
A conceptual diagram is an ERD in its simplest form. To create one, we only need two things: a table name and column headers.

It's simple because we're creating just the concept of the diagram. By covering only the basics, it's easier to capture the main points. If we tried to capture everything at once (data types, location of the primary and foreign keys, etc.), we're more likely to overlook a crucial item.



Logical Diagrams
Logical diagrams contain all of the same information that a conceptual diagram does, but the table is updated to include data types and primary keys.

Returning to the Quick DBD webpage, let's update our schema. Because we already took an initial look at the worksheet, we have already identified the primary key and know what type of data we're working with. Using the following syntax, update our Departments schema:

Add "varchar pk" to dept_no. Add "varchar" to dept_name. We use varchar (Links to an external site.) in these columns because the fields contain characters of varying length. Adding "pk" in the schema next to column indicates that column as a primary key. The table updated to reflect the changes in the text editor. A key symbol appears next to the dept_no line, indicating that it is the table's primary key, and varchar is added to indicate its type.
