# Employee Payroll System

This project is an Employee Payroll System implemented in Java using Object-Oriented Programming (OOP) concepts. The system allows you to manage and calculate the salaries of full-time and part-time employees.

## Features

- Add and remove employees.
- Calculate salaries for full-time and part-time employees.
- Display employee details.

## Classes and Methods

### Employee (Abstract Class)

- **Fields:**
  - `name` (String): The name of the employee.
  - `id` (int): The unique ID of the employee.
  
- **Methods:**
  - `Employee(String name, int id)`: Constructor to initialize the name and id.
  - `String getName()`: Returns the name of the employee.
  - `int getId()`: Returns the id of the employee.
  - `abstract double calculateSalary()`: Abstract method to calculate salary.
  - `String toString()`: Returns a string representation of the employee.

### FullTimeEmployee (Extends Employee)

- **Fields:**
  - `monthlySalary` (double): The monthly salary of the full-time employee.
  
- **Methods:**
  - `FullTimeEmployee(String name, int id, double monthlySalary)`: Constructor to initialize the name, id, and monthly salary.
  - `double calculateSalary()`: Returns the monthly salary.

### PartTimeEmployee (Extends Employee)

- **Fields:**
  - `hoursWorked` (int): The number of hours worked by the part-time employee.
  - `hourlyRate` (double): The hourly rate for the part-time employee.
  
- **Methods:**
  - `PartTimeEmployee(String name, int id, int hoursWorked, double hourlyRate)`: Constructor to initialize the name, id, hours worked, and hourly rate.
  - `double calculateSalary()`: Returns the salary calculated based on hours worked and hourly rate.

### PayrollSystem

- **Fields:**
  - `employeeList` (ArrayList<Employee>): A list to store employees.
  
- **Methods:**
  - `PayrollSystem()`: Constructor to initialize the employee list.
  - `void addEmployee(Employee employee)`: Adds an employee to the list.
  - `void removeEmployee(int id)`: Removes an employee from the list by id.
  - `void displayEmployees()`: Displays the details of all employees.
