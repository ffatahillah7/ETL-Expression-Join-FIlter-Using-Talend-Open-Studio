![image](https://github.com/user-attachments/assets/4f239e48-fba5-4efa-b66e-fab1d56cef1d)

# ETL Expression Join Filter Using tMap and tFilterRow Talend-Open-Studio
Extract data from PostgreSQL Databases, Transform using Expression, Join and Filter on tMap and tFilter Component Talend

The purpose of this project is to join several table using tMap component and filter the result using tFilterRow component.

Download Dataset file : [https://media.geeksforgeeks.org/wp-content/uploads/nba.csv](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce?resource=download)

## Goals of the Project:
1.  Extract data from PostgreSQL.
2.  Join several Table.
3.  Add and change column.
4.  Filter with specific value.

## Prerequisite
1.  Using Talend Open Studio for Big Data
2.  Using Java 11
3.  PostgreSQL on local computer

## Lesson Result
1.  Create connection on Metadata > Db Connection. This connection can used for open the data or table on any job in Talend.
2.  Open or exctract several table using tDBInput, checklist Use an existing connection, and choose tDBConnection that you have added before.
3.  Add tMap Component on workspace. Join several table just drag and drop the relational columns.
    Join Model    : Left Outer Join
    Match Model   : All Matches
4.  Add variable expression for get new columns or for change the exisiting columns. For example, getCurrentDate, StringHandling with Trim, upcase, lowercase, etc.
5.  Drag all the columns and Variable expression from source to destination. In destination window, we can add new column with calculation field.
6.  Add tFilterRow and choose the column to filter specific value.
7.  add tLogRow to display the result.
![image](https://github.com/user-attachments/assets/6767fbe3-63ec-49d3-9584-8777231fc3db)

