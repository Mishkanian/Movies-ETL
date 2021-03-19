# Movie Data - ETL in a Single Function

## Project Overview  
The purpose of this project is to create an automated pipeline that takes in new movie data, performs the appropriate transformations, and loads the data into existing tables. The existing code is refactored into one function that performs the ETL process.

## Resources and Software

- Python 3.7
- pgAdmin 4.50
- PostgreSQL v13

## Results  
The new ETL function performs correctly and the data is successfuly added to a PostgreSQL database. Please see the images below:

These outputs were created with the following queries:
```sql
SELECT COUNT(*) AS "Number of Movies row" FROM movies;
SELECT COUNT(*) AS "Number of Ratings row" FROM ratings;
```

**Author: Michael Mishkanian**  

For all questions and inquiries, please contact me on [LinkedIn](https://www.linkedin.com/in/michaelmishkanian/).
