# Crowdfunding Analysis

## Overview
We are working with some data for Independent Funding to create analysis of a crowdfunding Excel file using the ETL process. We have been provided a backer info file of crowdfunding information and will be using Python, Pandas and PostgreSQL to create specific output files for the client.

## Analysis Process
After extracting the data we cleaned the data into a usable dataset by dropping the name column and sorting the columns into five distinct columns shown below

![Cleaned_Columns](/Resources/Cleaned_Columns.png)

This allows us to export the data in a usable clean format for analysis in PostgreSQL

The next phase of our analysis will be to create a dataset that we can export the required information for the customer. The below diagram is how the SQL dataset is designed:

![Dataset](/Resources/crowdfunding_db_relationships.png)

The customer requested two distinct data analysis sets
- A table with email contacts that have a remaining goal
- A table with information about backers and remaining goal amounts

The first image shows the table schema of the first deliverable:

![contacts](/Resources/email_contacts_table.png)

And this is the table with the second deliverable:

![contacts](/Resources/email_backers_remaining_goal_amount.png)

Once these tables were created we exported the data in separate .csv files and provided them to the customer.