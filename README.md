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
ANSWER: SELECT * FROM CITY;
```
----
### Select by ID
###### Query all columns for a city in CITY with the ID 1661. The CITY table is described as follows:
![City Table](<SQL-CITY.jpg>)
```sql
ANSWER: select * from CITY where ID=1661;
```

----
### japanese cities attributes
###### Query all attributes of every Japanese city in the CITY table. The COUNTRYCODE for Japan is JPN. The CITY table is described as follows:
![City Table](<SQL-CITY.jpg>)
```sql
ANSWER: select * from CITY where COUNTRYCODE = 'JPN';
```
