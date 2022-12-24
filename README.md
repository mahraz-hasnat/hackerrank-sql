# SQL Preparation

### Revising the Select Query I
###### Query all columns for all American cities in the CITY table with populations larger than 100000. The CountryCode for America is USA. The CITY table is described as follows:
![City Table](<SQL-CITY.jpg>)
```sql
ANSWER: SELECT * FROM CITY WHERE POPULATION > 100000 AND COUNTRYCODE = "USA";
```
----
### Revising the Select Query II
###### Query the NAME field for all American cities in the CITY table with populations larger than 120000. The CountryCode for America is USA. The CITY table is described as follows:
![City Table](<SQL-CITY.jpg>)
```sql
ANSWER:  select NAME from CITY where POPULATION > 120000 and COUNTRYCODE = 'USA';
```

----
### Select All
###### Query all columns (attributes) for every row in the CITY table. The CITY table is described as follows:
![City Table](<SQL-CITY.jpg>)
```sql
ANSWER:  /*
    Enter your query here and follow these instructions:
    1. Please append a semicolon ";" at the end of the query and enter your query in a single line to avoid error.
    2. The AS keyword causes errors, so follow this convention: "Select t.Field From table1 t" instead of "select t.Field From table1 AS t"
    3. Type your code immediately after comment. Don't leave any blank line.
*/SELECT * FROM CITY;
```
