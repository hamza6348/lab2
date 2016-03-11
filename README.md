# CSV-file-reading-and-dataentry-into-database-usng-jdbc
Introduction:
In this lab we were given a CSV file which contained the data of cities and their longitude,latitude,postal code etc. a CSV File is a de-limiter separated file with a comma as a de-limiter. our task was to upload that data into a database using JDBC and then we have to search and return the city ,given the input by the user. he data is read line-by-line by our program

working: 
Instead of using the BufferedReader and other Java API directly, we use the open-csv library. The library reads the CSV File and provides us with a com.opencsv.CSVReader Object. The Reader.readNext() method in this class returns a String array for each row. This row can be iterated to extract field values and set them in the java.sql.PreparedStatement.
