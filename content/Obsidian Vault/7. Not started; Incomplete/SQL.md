2024-07-3119:57
Status: #Incomplete 

Manipulating data in Python E.x.=favorite show (data from Google survey)
```python
#Data processing 
#google forms (E.x.= favourite show) -> (convert to) excel -> csv file -> python
import csv

with open("favorites.csv", "r") as file:
    reader = csv.reader(file)
    next(reader)
#next skips the first row of the imported data
    for row in reader:
        print(row[1])
#prints out the first row (E.x.= favourite show title) 
```
```python
import csv
titles = []

with open("favorites.csv", "r") as file:
    reader = csv.DictReader(file)
#DictReader creates a dictionary from each row, allowing for access to each row by name
#DictReader uses the first row as the column names 
    for row in reader:
				title = row["title"].strip().upper() 
#.strip().upper() makes all titles upper case = canonicalized/standardized 
        if not row ["title"] in titles: 
						titles.append(row["title"])

for title in titles:
print(title) 
```

The most common way to save large amounts of information digitally is through the usage of databases. Similarly to programs like excel, databases are organized by a set of rows and columns.

SQL (the Structured Query Language) is the most powerful database program. Its purpose if to query a database. MySQL is one open-source platform on which you can establish the type of relational database that SQL is best at working at. SQLite is a less storage heavy version. Several installations of SQL come with a GUI(Graphical user interface) tool called phpMyAdmin which can be used to execute queries in a more user friendly way. It is most commonly used to create tables and databases as the syntax for making them is complicated. (You will be prompted to specify the columns of the table, then the majority of the queries executed will be on the rows )

storing in files/folders using python

Data types in SQL:

`[INT][SMALLINT][TINYINT][MEDIUMINT][BIGINT][DECIMAL][FLOAT][BIT][DATE][TIME]DATETIME][TIMESTAMP][CHAR = one character = fixed 1 string][VARCHAR][BINARY][BLOB][TEXT][ENUM][GEOMETRY = mapping data][LINESTRING = mapping data]…`

Primary keys enable rows of a table to be uniquely identified, (basically an index). You should have these values automatically increment as new information is being added (and be an int).

Joint primary keys are two columns that are always guaranteed to be unique

*SQL has very limited vocabulary

- SELECT extracts information from a table Use ’*’ to select all the columns (after `<columns>`)
- SELECT (JOIN) joins information across two different tables
- INSERT adds new information to the table
- UPDATE modifies information in a table

→ Other operations include: `[AVG][COUNT][COUNT][DISTINCT][LOWER][MAX][MIN][UPPER][WHERE][LIKE][ORDER BY][LIKE][GROUP BY]`
```sql
//**SELECT (JOIN)**
SELECT 
<columns>
FROM
<table1>
JOIN
<table2>
ON
<predicate>
```
```sql
//SELECT
SELECT <columns>
FROM 
<table>
WHERE <predicate>
ORDER BY 
<column>

```
```sql
//INSERT
INSERT INTO 
<table> 
(<columns>) 
VALUES 
(<values>)
```

```sql
//**UPDATE** 
UPDATE 
<table>
SET 
<column> = <value> 
WHERE
<predicate>
```
```sql
//DELETE 
DELETE FROM
<table>
WHERE
<predicate>
```

#### SQL Operations 

key =lambda
. = any character
.* = 0 or more characters
.+ = 1 or more characters
? = optional
^ = start of input
$ = end of input

relational database
create table table(column type, …);
.mode csv
.import
b tree
sequel attacks
?
rare conditions
atomic
interacting with databases at the same time as another user
