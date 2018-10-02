# This document specifies the steps to be taken to set-up a sample database for demo purposes.

The bacpac file (apimdemo_database_setup.bacpac) which is present in this folder will be used to setup the Sample database on an Azure SQL Database


a)  Upload the bacpac file(apimdemo_database_setup.bacpac) on a storage account container.
b)  Create an Azure SQL Server resource (If an Azure SQL Server already exists, this step can be omitted)
c)  Once the SQL Server is created, Navigate to SQL Server overview pane.
c)  Click Import database from the top menu.
d)  Select the storage account in which the file is uploaded, then select the file.
e)  Choose the pricing tier and other settings as per requirement.
f)  Click create and it will start to import the database from the file. 

g) Take note of the SQL Server connection for this database. This will be needed for doing the set-ups in the following steps of this demo


Reference Article : https://www.sqlshack.com/import-sample-bacpac-file-azure-sql-database/
