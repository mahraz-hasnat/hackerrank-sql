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
----
### Weather Observation Station 1
###### Query a list of CITY and STATE from the STATION table. The STATION table is described as follows:
![Station Table](<sql-station.jpg>)
```sql
ANSWER: select CITY , STATE from STATION;
```

----
### Weather Observation Station 3
###### Query a list of CITY names from STATION for cities that have an even ID number. Print the results in any order, but exclude duplicates from the answer The STATION table is described as follows:
![Station Table](<sql-station.jpg>)
```sql
ANSWER: select distinct CITY from STATION where mod(ID,2)=0 order by CITY asc;
```
----
### Weather Observation Station 5
###### Query the two cities in STATION with the shortest and longest CITY names, as well as their respective lengths (i.e.: number of characters in the name). If there is more than one smallest or largest city, choose the one that comes first when ordered alphabetically. The STATION table is described as follows:
![Station Table](<sql-station.jpg>)
```sql
ANSWER: select CITY, length(CITY) from STATION where length(CITY) = (select min(length(CITY)) from STATION ) order by CITY ASC LIMIT 1;
select CITY, length(CITY) from STATION where length(CITY) = (select max(length(CITY)) from STATION ) order by CITY ASC LIMIT 1;
```
