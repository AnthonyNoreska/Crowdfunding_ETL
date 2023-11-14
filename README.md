# Crowdfunding_ETL
Crowdfunding Data Management Project

Project Overview
This project involves organizing crowdfunding-related data by creating Category, Subcategory, Campaign, and Contacts datasets. Additionally, a PostgreSQL database is established to efficiently manage and analyze the data. 

Project Steps
1. Category and Subcategory DataFrames
	a. Category DataFrame
* Created a DataFrame with a "category_id" column going sequentially from "cat1" to "catn."
* Included a "category" column containing only category titles.
* Exported the category DataFrame as category.csv and saved it to the GitHub repository.
	b. Subcategory DataFrame
* Created a DataFrame with a "subcategory_id" column going sequentially from "subcat1" to "subcatn."
* Included a "subcategory" column with only subcategory titles.
* Exported the subcategory DataFrame as subcategory.csv and saved it to the GitHub repository.

2. Campaign DataFrame
* Created a DataFrame with the following columns:
* "cf_id"
* "contact_id"
* "company_name"
* "description" (renamed from "blurb")
* "goal" (converted to float)
* "pledged" (converted to float)
* "outcome"
* "backers_count"
* "country"
* "currency"
* "launch_date" (formatted as "YYYY-MM-DD")
* "end_date" (formatted as "YYYY-MM-DD")
* "category_id" (matching those in the Category DataFrame)
* "subcategory_id" (matching those in the Subcategory DataFrame)
* Exported the campaign DataFrame as campaign.csv and saved it to the GitHub repository.

3. Contacts DataFrame
* Imported the contacts.xlsx file into a DataFrame.
* Utilized Python dictionary methods to create a new DataFrame with "contact_id," "first_name," "last_name," and "email" columns.
* Split the "name" column into first and last names.
* Exported the contacts DataFrame as contacts.csv and saved it to the GitHub repository.

4. Crowdfunding Database
	a. Database Schema
* Sketched an Entity-Relationship Diagram (ERD) for the tables using QuickDBD or a similar tool.
* Created a table schema for each CSV file, specifying data types, primary keys, foreign keys, and other constraints.
* Saved the database schema as a PostgreSQL file named crowdfunding_db_schema.sql and saved it to the GitHub repository.
	b. Database Creation
* Created a new PostgreSQL database named crowdfunding_db.
* Used the information from the crowdfunding_db_schema.sql file to create tables in the correct order, considering foreign keys and relationships.
* Verified the table creation by running a SELECT statement for each table.
	c. Data Import
* Imported each CSV file into its corresponding SQL table in the crowdfunding_db database.
* Verified that each table has the correct data by running a SELECT statement for each.


Conclusion
The project successfully transformed crowdfunding data into structured CSV files and a PostgreSQL database, facilitating efficient data management and analysis. If further clarification is needed, refer to the project steps or seek assistance from the instructional team.

