![image](https://github.com/user-attachments/assets/b809676c-01b5-4f08-a5fc-796a946ee316)


# ETL Expression, Join, Filter, and multiple output Using tMap and tFilterRow Talend-Open-Studio
Extract data from PostgreSQL Databases, Transform using Expression, Join and Filter on tMap and tFilter Component Talend, add multiple output for data warehouse or datamart.

The purpose of this project is to join several table using tMap component and filter the result using tFilterRow component.

Download Dataset file : [https://media.geeksforgeeks.org/wp-content/uploads/nba.csv](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce?resource=download)

## Goals of the Project:
1.  Extract data from PostgreSQL.
2.  Join several Table.
3.  Add and change column.
4.  Filter with specific value.
5.  Store multiple output based on tFilterRow to data warehouse or data mart.

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
4.  Add variable expression for get new columns or for change the exisiting columns. For example, getCurrentDate, StringHandling with Trim, upcase, lowercase, etc. We can add multiple output on output window tMap.
5.  Drag all the columns and Variable expression from source to destination. In destination window, we can add new column with calculation field.
6.  Add multiple tFilterRow and choose the column to filter specific value.
7.  add multiple tLogRow to display the result. We can also add database output to store the result to data warehouse or data mart.
   
![image](https://github.com/user-attachments/assets/db99bf6a-0dcc-4db9-b3d5-58a0fbef5ac4)


