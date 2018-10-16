# This document specifies the steps to be taken to set-up a sample Azure Api App for this demo purposes.

The code/solution in the SoapWebAPI.rar file which is present in this folder will be used to setup the Azure Api App.

This was chosen as an example API to demonstrate how APIM could integrate with varied kinds of backend services


a)  Navigate to Azure portal and create a new API App hosted in App Service Plan.
b)  Unzip/uncompress the SoapWebAPI.rar file which was provided as part of the 'Azure Api App' folder
c)  Now open the .sln file into Visual Studio and modify the connection string in web.config file present inside 'Views' folder.
    The myconnectionstring property in the web.config is the one which needs to be modified
d)  Once the connection string is modified, build the code
e)  Now publish this solution to the API app created as step 1.
f)  Test the Azure Api App is working independently. To test the Azure Api App, Goto the URL from the Azure portal and test the App is live (Replace the App APi Name in below)

https://<<ApiAppName>>.azurewebsites.net/Order

Reference Article : https://www.c-sharpcorner.com/article/azure-app-service-api-apps/ 
