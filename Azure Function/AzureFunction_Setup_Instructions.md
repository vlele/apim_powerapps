# This document specifies the steps to be taken to set-up a sample Azure Function for this demo purposes.

The code in the GetProducts.txt file which is present in this folder will be used to setup the Azure Function


a)  Create a Function App in the required subscription, resource group and location.
b)  Once the Azure Function is created, Add the Connection String in Application Settings, which can be found in Platform Features of the Azure Function.
	This is the connection string to the database which was created in the Database Setup.
c)  Now, add a new function and select its trigger as HTTP.
d)  Replace the code provided in GetProjects.txt into run.csx file and click save
    (This code is specific for this demo)
e)  Test the Azure Function is working independently. To test the Azure function, paste the below in the request body and run the Azure function.

{
    "ProductId": ""
} 



Reference Article : https://visualstudiomagazine.com/articles/2017/04/01/http-triggered-functions.aspx
