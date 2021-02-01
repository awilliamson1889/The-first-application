# <center>Personnel management</center>
***
## 1.Introduction
### 1.1 Purpose
The purpose of this document is to provide a detailed description of the web application "Personnel management".
It will explain the purpose of the web application, what it will do and the limitations under which it will work.
This document is intended for users of the application, as well as for potential developers.
### 1.2 Product Scope
"Personnel management" is a web application that can be used to manage employees and departments in an organization.
***
## 2.Overall Description
### 2.1 Product perspective
"Personnel management" is a web application that implements a client-server interaction model. "Personnel management" provides the user with a simple mechanism for working with a database that contains information about the organization. When processing user requests, the application displays or manipulates data in the database.
### 2.2 Product functions
With this web application, the user can manage the employees and departments of the organization. The user has access to two tables that store all the necessary information. Data manipulation functions such as adding, deleting, and editing are available to the user.
Also, for the convenience of working with tables in this web application, there is a table search and filtering.
***
## 3.Specific requirements
### 3.1 User interfaces
"Personnel management" - is a web application that automates the management of employees and departments in an organization.
The application must provide:

- Displaying information about employees/departments;
- Adding new employees/department;
- Editing employee/department information;
- Deletion of information about employees.
### 3.2 Employees
#### 3.2.1 Display list of employees
This page displays a table of the organization's employees. Also on this page there is a search by name and a filter by department.

***Main scenario:***

+ User selects item “Employees”;
+ Application displays list of Employees.

<img src="https://github.com/awilliamson1889/The-first-application/blob/main/documentation/pictures/Employees.png"  width="600" height="600">

Pic. 3.2.1 View the Employees list.


The list displays the following columns:
+ Name – employee name;
+ Surname – employee surname;
+ Department – employee department;
+ Date of Birth – employee date of birth;
+ Salary – employee salary;

***Filtering by department:***
+ In the employees list view mode, the user sets a department filter;
+ The application will display a form to view the list of employees with updated data. 

#### 3.2.2 Add employee
 Main scenario:
+ User clicks the “Add employee” button in the employees list view mode;
+ Application displays form to enter employee data;
+ User enters employee data and presses “Save” button;
+ If a user clicks on the new button, they are redirected to the department creation page;
+ If any data is entered incorrectly, incorrect data messages are displayed;
+ If entered data is valid, then record is adding to database;
+ If error occurs, then error message is displaying;
+ If new employee record is successfully added, then list of employees with added records is displaying.

Cancel operation scenario:
+ User clicks the “Add employee” button in the employees list view mode;
+ Application displays form to enter employee data;
+ User enters employee data and presses “Cancel” button;
+ Data don’t save in data base, then list of employees records is displaying to user;
+ If the user selects the menu item "Employees” or "Departments", the data will not be saved to the
database and the corresponding form with updated data will be opened.

<img src="https://github.com/awilliamson1889/The-first-application/blob/main/documentation/pictures/Add%20Employee.png"  width="600" height="600">

Pic. 3.2.2 Add employee.

When adding a employee, the following details are entered:
+ Name – employee name;
+ Surname – employee surname;
+ Department – employee department;
+ Date of Birth – employee date of birth;
+ Salary – employee salary;

#### 3.2.3 Edit employees
 Main scenario:
+ User clicks the “Edit” button in the employees list view mode;
+ Application displays form to enter employee data;
+ User enters employee data and presses “Save” button;
+ If a user clicks on the new button, they are redirected to the department creation page;
+ If any data is entered incorrectly, incorrect data messages are displayed;
+ If entered data is valid, then record is adding to database;
+ If error occurs, then error message is displaying;
+ If new employee record is successfully added, then list of employees with added records is displaying.

Cancel operation scenario:
+ User clicks the “Add employee” button in the employees list view mode;
+ Application displays form to enter employee data;
+ User enters employee data and presses “Cancel” button;
+ Data don’t save in data base, then list of employees records is displaying to user;
+ If the user selects the menu item "Employees” or "Departments", the data will not be saved to the
database and the corresponding form with updated data will be opened.

<img src="https://github.com/awilliamson1889/The-first-application/blob/main/documentation/pictures/Add%20Employee.png"  width="600" height="600">

Pic. 3.2.3 Edit employee.

When adding a employee, the following details are entered:
+ Name – employee name;
+ Surname – employee surname;
+ Department – employee department;
+ Date of Birth – employee date of birth;
+ Salary – employee salary;

Constraints for data validation:
+ Name – maximum length of 90 characters;
+ Surname – maximum length of 90 characters;
+ Date of Birth – order add date in format dd/mm/yyyy;
+ Salary – non-negative number.

#### 3.2.4 Delete employees
Main scenario:
+ The user, while in the list of employees, presses the "Delete" button in the selected employee line;
+ If the employee can be removed, a confirmation dialog is displayed;
+ The user confirms the removal of the employee;
+ Record is deleted from database;
+ If error occurs, then error message displays;
+ If employee record is successfully deleted, then list of employees without deleted records is displaying.

<img src="https://github.com/awilliamson1889/The-first-application/blob/main/documentation/pictures/Delete%20Employee.png"  width="600" height="600">

Pic. 3.2.4 Delete employee.

 Cancel operation scenario:
+ User is in display mode of employees list and press “Delete” button;
+ Application displays confirmation dialog “Please confirm delete employee?”;
+ User press “Cancel” button;
+ List of employees without changes is displaying. 

#### 3.2.5 View employee information
Main scenario:
+ User is in display mode of employees list and press “View” button;
+ Application displays information page.

<img src="https://github.com/awilliamson1889/The-first-application/blob/main/documentation/pictures/View%20Employee.png"  width="600" height="600">

Pic. 3.2.5 Information about employee.

### 3.3 Departments
#### 3.3.1 Display list of departments
This page displays a table of the organization's departments. Also on this page there is a search by department name.

***Main scenario:***

+ User selects item “Departments”;
+ Application displays list of Departments.

<img src="https://github.com/awilliamson1889/The-first-application/blob/main/documentation/pictures/Departments.png?"  width="600" height="600">

Pic. 3.3.1 View the Departments list.


The list displays the following columns:
+ Department – department name;
+ Total Employees – number of employees.

#### 3.3.2 Add department
 Main scenario:
+ User clicks the “Add department” button in the departments list view mode;
+ Application displays form to enter department data;
+ User enters department data and presses “Save” button;
+ If any data is entered incorrectly, incorrect data messages are displayed;
+ If entered data is valid, then record is adding to database;
+ If error occurs, then error message is displaying;
+ If new department record is successfully added, then list of departments with added records is displaying.

Cancel operation scenario:
+ User clicks the “Add department” button in the departments list view mode;
+ Application displays form to enter department data;
+ User enters department data and presses “Cancel” button;
+ Data don’t save in data base, then list of departments records is displaying to user;
+ If the user selects the menu item "Employees” or "Departments", the data will not be saved to the
database and the corresponding form with updated data will be opened.

<img src="https://github.com/awilliamson1889/The-first-application/blob/main/documentation/pictures/Add%20Department.png"  width="600" height="600">

Pic. 3.3.2 Add department.

When adding a employee, the following details are entered:
+ Department – department name.

#### 3.3.3 Edit department
 Main scenario:
+ User clicks the “Edit” button in the departments list view mode;
+ Application displays form to enter department data;
+ User enters department data and presses “Save” button;
+ If any data is entered incorrectly, incorrect data messages are displayed;
+ If entered data is valid, then record is adding to database;
+ If error occurs, then error message is displaying;
+ If new department record is successfully added, then list of departments with added records is displaying.

Cancel operation scenario:
+ User clicks the “Add department” button in the departments list view mode;
+ Application displays form to enter department data;
+ User enters employee data and presses “Cancel” button;
+ Data don’t save in data base, then list of departments records is displaying to user;
+ If the user selects the menu item "Employees” or "Departments", the data will not be saved to the
database and the corresponding form with updated data will be opened.

<img src="https://github.com/awilliamson1889/The-first-application/blob/main/documentation/pictures/Add%20Department.png"  width="600" height="600">

Pic. 3.3.3 Edit department.

When adding a department, the following details are entered:
+ Department – department name.

Constraints for data validation:
+ Department – unique value.

#### 3.3.4 Delete department
Main scenario:
+ The user, while in the list of departments, presses the "Delete" button in the selected department line;
+ If the department can be removed, a confirmation dialog is displayed;
+ The user confirms the removal of the department;
+ Record is deleted from database;
+ If error occurs, then error message displays;
+ If department record is successfully deleted, then list of departments without deleted records is displaying.

<img src="https://github.com/awilliamson1889/The-first-application/blob/main/documentation/pictures/Delete%20Department.png"  width="600" height="600">

Pic. 3.3.4 Delete department.

 Cancel operation scenario:
+ User is in display mode of departments list and press “Delete” button;
+ Application displays confirmation dialog “Please confirm delete department?”;
+ User press “Cancel” button;
+ List of departments without changes is displaying. 

