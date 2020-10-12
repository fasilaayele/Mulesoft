# Mulesoft

MS3 Contact API- Database Implementation project
home
This template helps you design an Employee System API. It provides a means of hiding the complexity of the database implementation from a user while exposing data in a canonical format. The template abstracts Employee data from a database.

Operations
The MS3 Contact API supports the following operations:
      GET /employees/employee
      POST /employees/employee
      PUT /employees/employee
      DELETE /employees/employee
      
Use Case
This template serves as a foundation for the API led connectivity approach of running an enterprise.
The template is a system API to an underlying MySql database.
This template is a REST API implemented using APIkit and RAML definition. The basic operations are implemented for a single employee record. The API uses JSON as an exchange format. Included are example requests and responses.


Assumption
Employee records are assumed unique by First name and Last name and retrieves employee records from database based on the combination of query parameters.

Client_id and client_secrete should be included in the header during running the test.


GET /Employees/Employee
Retrieves employee record from a database based on the combination of query parameters. 
POST /Employees/Employee
Inserts a new employee record in a database.
PUT /Employees/Employee
Update employee record from a database.
DELETE /Employees/Employee
Deletes employee record from a database based on the combination of query parameters. 
Considerations
To make this template run, there are certain preconditions that must be considered. All of them deal with the preparations, that must be made for all to run smoothly. 

This implementation requires a database instance to work. 

Running on Studio
After you import the project into Anypoint Studio, follow these steps to run it:
•	Locate the properties file properties.yaml, in src/main/resources.
http:
  port: "8081"
db:
  host: "mudb.learn.mulesoft.com"
  port: "3306"
  user: "mule"
  password: "mule"
  database: "training"
•	Complete all the properties required as per the examples in the "Properties to Configure" section.
•	Right click the template project folder.
•	Hover your mouse over Run as.
•	Click Mule Application (configure).
•	Inside the dialog, select Environment and set the variable mule.Env to the value dev.
•	Click Run.
Deploying a Project in CloudHub
In Studio, right click your project name in Package Explorer and select Anypoint Platform > Deploy on CloudHub.
Properties to Configure
To use this project, you need to configure some properties (Credentials, configurations, etc.) either in properties.yaml file or in CloudHub as Environment Variables. 
