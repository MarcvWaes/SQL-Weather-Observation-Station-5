# SQL-Weather-Observation-Station-5

# Challenge:
- Query the two cities in STATION with the shortest and longest CITY names, as well as their respective lengths (i.e.: number of characters in the name). If there is more than one smallest or largest city, choose the one that comes first when ordered alphabetically.

- The STATION table is described as follows:

![n1e5uock jot](https://github.com/MarcvWaes/SQL-Weather-Observation-Station-3/assets/120553175/93033af8-77bd-460d-bf7b-fce39386b9e6)

- Where LAT_N is the northern latitude and LONG_W is the western longitude.

# Solution:
- SELECT CITY AS C, LENGTH(CITY) AS L
- FROM STATION
- ORDER BY L DESC, C ASC
- LIMIT 1;

- SELECT CITY AS C, LENGTH(CITY) AS L
- FROM STATION
- ORDER BY L ASC, C ASC
- LIMIT 1;

# Output:
- Marine On Saint Croix 21
- Amo 3
