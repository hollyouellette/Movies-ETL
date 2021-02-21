# Movies Extract > Transform > Load

## Project Brief 

This project was completed to assist Amazing Prime Video in developing an algorithm to predict which low-budget movies being released will become popular so that they can buy the streaming rights.

In order to accomplish this, Amazing Prime Video will be hosting a hackathon whereby teams of analysts will collaborate and work intensively with data from movies released since 1990.

This repository contains the following: 

   1. A Resources folder containing the raw datasets that were gathered from Wikipedia and Kaggle.<br><br/>
   2. Four deliverables focused on extracting, transforming and loading the multiple data sources into a SQL database so that the Hackathon participants have a clean dataset to work with:<br><br/>
        **Deliverable 1** <a href="https://github.com/hollyouellette/Movies-ETL/blob/main/ETL_function_test.ipynb/" target="_blank">ETL_function_test.ipynb</a> <br/>
         This file contains a completed function that reads in the three data files and creates three separate DataFrames.<br/><br/>
         **Deliverable 2** <a href="https://github.com/hollyouellette/Movies-ETL/blob/main/ETL_clean_wiki_movies.ipynb">clean_wiki_movies.ipynb</a> <br/>
         This file contains the completed code to extract and transform the Wikipedia data so that it is ready to merge with the Kaggle metadata. <br><br/>
         **Deliverable 3** <a href="https://github.com/hollyouellette/Movies-ETL/blob/main/ETL_clean_kaggle_data.ipynb">ETL_clean_kaggle_data.ipynb</a><br/>
         In this file, Kaggle metadata and MovieLens rating data are extracted and transformed, then converted into separate DataFrames. Next, the two DataFrames are merged into one movies_df Dataframe. Finally, the movies_df Dataframe is merged with the MovieLens rating data DataFrame to create movies_with_ratings_df.<br><br/>
         **Deliverable 4** <a href="https://github.com/hollyouellette/Movies-ETL/blob/main/ETL_create_database.ipynb">ETL_create_database</a><br/>
         In this final deliverable, the previous code was refactored to add the movies_df Dataframe and MovieLens rating data to a SQL database. See the final row counts from PostgreSQL the images below: <br><br/>
 
<img src="https://github.com/hollyouellette/Movies-ETL/blob/main/Resources/movies_query.png" align=center width=450>
<img src="https://github.com/hollyouellette/Movies-ETL/blob/main/Resources/ratings_query.png" align=center width=450>
