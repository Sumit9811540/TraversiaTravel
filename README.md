
# Employee Management System

## Project Overview

This project is a simple **ASP.NET Core MVC** application connected with **SQL Server**.

### Key Features:
- **User Login**: Static username/password check for authentication.
- **User Management**: Displays a list of users stored in the database.
- **Pagination**: Only 10 users shown per page with navigation for additional pages.

## Database Design

### Database: `EmployeeDB`

#### Table: `Users`

| Column  | Data Type    | Constraints                                |
|---------|--------------|--------------------------------------------|
| Id      | INT          | Primary Key, Identity                     |
| Name    | NVARCHAR(50) | NOT NULL                                   |
| Email   | NVARCHAR(100)| NOT NULL, UNIQUE                          |
| Mobile  | CHAR(10)     | NOT NULL, UNIQUE                          |
| Gender  | NVARCHAR(10) | NOT NULL                                   |
| Address | NVARCHAR(200)| NOT NULL                                   |

## Connection String

The project uses **SQL Server Local Instance** with the following connection string:

```plaintext
Data Source=DESKTOP-0LSS3AS\SQLEXPRESS01;Initial Catalog=EmployeeDB;Integrated Security=True
````

## Login Details

* **Username**: `sumit`
* **Password**: `admin`

**Note**: The user must log in successfully to access the User List page.

## Features

### 1. User Login

* Simple login form with username and password fields.
* Redirects to the User List page upon successful login.
* Displays an error message for incorrect credentials.

### 2. User List

* Displays users stored in the `Users` table.
* Shows 10 records per page, with next/previous page navigation for additional records.

## Technology Stack

* **Backend**: ASP.NET Core MVC (.NET 8)
* **Database**: SQL Server 2019 (EmployeeDB)
* **Language**: C#
* **Frontend**: Razor Views (HTML, CSS, Bootstrap)

## Future Enhancements

* Add User Registration with form validation.
* Implement Edit/Delete functionality for users.
* Implement Authentication & Authorization using ASP.NET Identity.
* Add Search and Filter options in the User List.

```
```
