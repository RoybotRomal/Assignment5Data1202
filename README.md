# Assignment5Data1202
Assignment 5, creating Github repository
The first part of the code imports necessary libraries including NumPy, Pandas, SQLAlchemy, and PyMySQL.
The next line of code reads a CSV file ('youtube_dataset.csv') into a Pandas DataFrame ('df_youtube') using the 'read_csv' function.
The 'head' function is then used to preview the first 5 rows of the 'df_youtube' DataFrame.
The 'info' function is used to display information about the DataFrame such as the column names, data types, and non-null count.
The 'df_first_1000_rows' DataFrame is created by selecting the first 1000 rows of the 'df_youtube' DataFrame.
The 'distribution' function is defined to get the distribution of a specified column in a DataFrame.
The 'df_dist' DataFrame is created by calling the 'distribution' function with the 'df_first_1000_rows' DataFrame and the 'channeltype' column name.
The 'df_first_1000_rows' DataFrame is then saved to a CSV file named 'youtube_top_1000.csv'.
An SQLAlchemy engine is created with the database connection details using 'create_engine' function.
The 'df_10' DataFrame is created by selecting the first 10 rows of the 'df_first_1000_rows' DataFrame.
The 'df_10' DataFrame is then written to a MySQL database table named 'df_10' using the 'to_sql' function. The column data types are specified using the 'dtype' parameter. If the 'if_exists' parameter is set to 'replace', it replaces the existing table with the same name, if any.
