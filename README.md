# NIQ-GFK-Assignment
I have completed the assingement in following stages.
1. Loaded the movies.dat file and created movies_raw_df.
2. Extracted the 'Year' from 'Title' and created a new column for the same. Also exploded the 'Genres' column which was having multiple values seprated by '|'.
3. Created a new df called movies_df and unpersisted the intermidiate df movies_raw_df.
4. Created users_raw_df from users.dat file.
5. Filtered users by non-null zip code and age range 18-59 and created a new df users_df, unpersisted users_raw_df.
6. Created ratings_df from ratings.dat file.
7. Joined ratings with movies, filtered movies released after 1989, grouped by genre and year, and calculated average rating in average_ratings_df.
8. Unpersisted df movies_df, users_df, ratings_df.
9. Aditionally, I created delta table on the cleaned and aggregated data, partitioned by generes to speed up the queries on the data.
10. Finally tried to query the data from delta table based on certain Genre.
