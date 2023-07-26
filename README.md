Employee Management Service
This service is a basic RESTful web service built using Spring Boot. It allows for the management of a list of employees, supporting operations to get the list of employees, add a new employee, and delete an existing employee.

Project Structure
DemoApplication: The entry point to the application. The main method in this class launches the Spring Boot application.

Employee: This class represents an Employee entity with properties such as id, firstName, lastName, and email.

Employees: This class is a container for a list of Employee objects.

EmployeeDAO: This class handles the data operations on the Employee objects.

EmployeeController: This class is a web controller that handles HTTP requests and responses.

How to Run the Application
To run this application, you will need to:

Clone the repository to your local machine.
Navigate to the project directory.
Run mvn spring-boot:run or ./mvnw spring-boot:run (if you're using the Maven wrapper) to start the application.
Interacting with the Service
Once the application is up and running, you can interact with the service using curl command or tools like Postman.

Get a list of all employees
Navigate to http://localhost:8080/employees.

Add an Employee
To add an employee, run the following curl command:

curl -X POST -H "Content-Type: application/json" -d '{"firstName": "John", "lastName": "Doe", "email": "john.doe@example.com"}' http://localhost:8080/employees
Delete an Employee
To delete an employee, run the following curl command:

curl -X DELETE http://localhost:8080/employees/1
Replace 1 with the id of the employee you wish to delete.

Contributing
Feel free to fork this repository and contribute. All pull requests are welcome.

Feel free to modify this 
