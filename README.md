# Pipeline-project
Capstone project 1: Census Data Standardization and Analysis Pipeline
Census Data Processing and Analysis
Problem Statement
The task involves cleaning, processing, and analyzing census data sourced from a specific dataset. This includes renaming columns for uniformity, handling missing data, standardizing state/UT names, accommodating new state formations, storing data, establishing database connections, and performing queries for further analysis and visualization.

Tasks
Task 1: Rename Column Names
To ensure consistency and reflect the census year, rename specific columns as follows:

State name to State/UT
District name to District
Male_Literate to Literate_Male
Female_Literate to Literate_Female
Rural_Households to Households_Rural
Urban_Households to Households_Urban
Age_Group_0_29 to Young_and_Adult
Age_Group_30_49 to Middle_Aged
Age_Group_50 to Senior_Citizen
Age not stated to Age_Not_Stated
Task 2: Rename State/UT Names
Standardize State/UT names:

Convert all caps to proper case format (first letter uppercase, rest lowercase).
Special case: Convert "and" to all lowercase.
Task 3: New State/UT Formation
Handle new state/UT formations:

In 2014, rename "Andhra Pradesh" to "Telangana" for specified districts.
In 2019, rename "Jammu and Kashmir" to "Ladakh" for specified districts.
Task 4: Find and Process Missing Data
Identify and process missing data:

Calculate and store the percentage of missing data for each column.
Use available data (e.g., population, literacy) to infer and fill missing values where possible.
Task 5: Save Data to MongoDB
Save processed data to MongoDB:

Store the cleaned and processed census data in a MongoDB collection named "census".
Task 6: Database Connection and Data Upload
Connect to a relational database and upload data:

Fetch data from MongoDB and upload it to a relational database using Python.
Use file names (without extensions) as table names.
Define primary key and foreign key constraints as necessary.
Task 7: Run Query on the Database and Show Output on Streamlit
Perform database queries and visualize results:

Execute queries on the relational database.
Display query results dynamically using Streamlit for interactive visualization.
Tools and Technologies
Python: Pandas, pymongo, SQLAlchemy, Streamlit
Databases: MongoDB, PostgreSQL (or other relational database)
File Handling: CSV, Excel

