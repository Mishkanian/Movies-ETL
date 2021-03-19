# Movie Data - ETL in a Single Function

## Project Overview  
The purpose of this project is to create an automated pipeline that takes in new movie data, performs the appropriate transformations, and loads the data into existing tables. The existing code is refactored into one function that performs the ETL process.

## Resources and Software

- Resources:
  - [Wikipedia Movie Data](https://github.com/Mishkanian/Movies-ETL/blob/main/Resources/wikipedia-movies.json)
  - Kaggle Movie Data: The file size of this data exceeds the maximum size allowed on GitHub. However, you may [download it directly from Kaggle](https://www.kaggle.com/rounakbanik/the-movies-dataset).
    - In the zip file downloaded from Kaggle, only **"movies_metadata.csv"** and **"ratings.csv"** are used in this project.
- Python 3.7
- pgAdmin 4.50
- PostgreSQL v13

## Results  
The new ETL function performs correctly and the data is successfuly added to a PostgreSQL database as seen in the images below. The final code can be viewed [here](https://github.com/Mishkanian/Movies-ETL/blob/main/ETL_create_database.ipynb).

![movie](https://github.com/Mishkanian/Movies-ETL/blob/main/Resources/movies_row.png)

![ratings](https://github.com/Mishkanian/Movies-ETL/blob/main/Resources/ratings_rows.png)

These outputs were created with the following queries:
```sql
SELECT COUNT(*) AS "Number of Movies row" FROM movies;
SELECT COUNT(*) AS "Number of Ratings row" FROM ratings;
```

**Author: Michael Mishkanian**  

For all questions and inquiries, please contact me on [LinkedIn](https://www.linkedin.com/in/michaelmishkanian/).
