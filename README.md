# Digital-Prescription-Analysis
Digital-Prescription-Analysis is an ETL project using Python and MySQL. It extracts prescription data from CSVs, cleans and transforms it, loads it into a database, and visualizes insights like top medicines, doctor performance, trends, and outliers.

# Step 1 : Installing Required Libraries
pandas

mysql.connector

matplotlib

sqlalchemy

urllib.parse

# Extract
# Step 2 : Reading from datasets
We have reading four datasets listed below
doctors
patients
medicines
prescriptions

# Transform
# Step 3 : Data Cleaning
While doing data cleaning , I was used all the methods.
Removing dupicates by -- drop_duplicates() method.
Handling missing values by -- fillna() method.
Converted dates by -- to_datetime() method.

# Load
# Step 4 : Connecting to MySQL and Creating datbase
By using my MySQL Login details ,i was created the connection by sqlalchemy.
and also i was created database by using connect() and execute methods of sql.

# Step 5 : Creating Tables
I was created all the table by using SQL Queries, and executed all the statement safely by connect() and execute() method.

# Step 6 : Storing cleaned data into MySQL
By using to_sql() method ,i was push all the cleaned data to MySQL server.

# Step 7 : Analytical Queries for Business Problems
# Most Prescribed medicines
<img width="860" height="486" alt="image" src="https://github.com/user-attachments/assets/a2b2803e-46e8-4ea0-a9fb-c2d3f278be30" />

# Doctors by Prescription Volume
<img width="861" height="482" alt="image" src="https://github.com/user-attachments/assets/2f11d541-061f-4aa0-8aca-f43a4978f4e3" />

# Gender-wise prescription distribution
<img width="442" height="352" alt="image" src="https://github.com/user-attachments/assets/98b79fab-4aec-4a8c-868b-a826e19f958d" />

# Age group vs number of prescriptions
<img width="892" height="480" alt="image" src="https://github.com/user-attachments/assets/585a8c68-f0a7-41d6-ad21-5c9d4083a5c7" />

# Doctor Prescription Count (Outlier Detection)
<img width="893" height="481" alt="image" src="https://github.com/user-attachments/assets/40e5f504-36d5-4c93-9155-9b0797078bf8" />

# Daily prescription trend over time
<img width="883" height="435" alt="image" src="https://github.com/user-attachments/assets/bb81e6b9-105a-4732-909b-28787b946267" />

# Missing data impact analysis before vs after cleaning.
<img width="886" height="607" alt="image" src="https://github.com/user-attachments/assets/0dec1388-9ad8-462e-be6b-65b06e79742b" />

# Conclusion 
The Digital Prescription Record Analysis system provides an efficient and structured way to manage doctors, patients, medicines, and prescriptions using a MySQL database. It ensures accurate record maintenance, reduces manual errors, and improves data accessibility for better healthcare management. Overall, the project demonstrates how database design and data analysis techniques can enhance operational efficiency and support informed decision-making in medical systems.

