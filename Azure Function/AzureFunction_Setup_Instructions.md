# This document specifies the steps to be taken to set-up a sample Azure Function for this demo purposes.

The code in the GetProducts.txt file which is present in this folder will be used to setup the Azure Function


a)  Create a Function App in the required subscription, resource group and location.
b)	Once the azure function is created, navigate to Function App settings and change the Runtime version to ~1. As per latest changes in Azure Function Apps, default version selected is ~2. (This sample is only compatible with Azure Function 1.0)
c)  Add the Connection String in Application Settings, which can be found in Platform Features of the Azure Function.
	This is the connection string to the database which was created in the Database Setup.
d)  Add a new function and select its trigger as HTTP.
e)  Open the Files section inside the function app and create a new file with the name, project.json and paste the content of project.json file present in the Azure Function folder.
	This will install the required dependencies for function code. To verify installation of required packages, check the logs in the function app.
	Alternately you could directly upload the project.json file in the repository to the Azure Function.
f)	Replace the code provided in GetProjects.txt into run.csx file and click save
    (This code is specific for this demo)
g)  Test the Azure Function is working independently. To test the Azure function, paste the below in the request body and run the Azure function.

{
    "ProductId": ""
} 



Reference Article : https://visualstudiomagazine.com/articles/2017/04/01/http-triggered-functions.aspx
