# Master-Details Core API CRUD Application - Employee Management

Welcome to the **Master-Details Core API CRUD Application**! This ASP.NET Core Web API project efficiently manages employee data along with associated details such as job history, project assignments, and dependents, utilizing a master-details structure.

## Table of Contents

- [✨ Key Features](#key-features)
- [🛠️ Tech Stack](#tech-stack)
- [🚀 Getting Started](#getting-started)
- [📦 Installation](#installation)
- [🖥️ Usage](#usage)
- [📄 API Documentation](#api-documentation)
- [👤 Example Use Cases](#example-use-cases)
- [🤝 Contributing](#contributing)
- [📄 License](#license)
- [📬 Contact](#contact)

## ✨ Key Features

### Employee Management (Master)
- **CRUD Operations**: Create, read, update, and delete employee records with fields such as:
  - `EmployeeID`
  - `Name`
  - `Position`
  - `Department`
  - `HireDate`

### Details Management
- **Job History**: Maintains records of an employee’s previous positions, departments, and durations.
- **Project Assignments**: Tracks projects assigned to employees, including:
  - `ProjectID`
  - `Role`
  - `Duration`
- **Dependents**: Manages associated dependents, detailing:
  - `DependentName`
  - `Relationship`
  - `DateOfBirth`

Each detail entity supports CRUD operations for managing related records.

### Cascade Operations
- Implement cascade delete/update options to manage related records in job history, projects, or dependents when deleting an employee.

### DTOs (Data Transfer Objects)
- Create DTOs for optimized data transfer and to hide sensitive information.

## 🛠️ Tech Stack

- **ASP.NET Core Web API**: For creating RESTful endpoints to handle CRUD operations on employees and related details.
- **Entity Framework Core**: For managing relationships between the Employee (master) and related details tables (JobHistory, ProjectAssignments, Dependents).
- **Database**: SQL Server, PostgreSQL, or MySQL for structured storage of employee and related data.
- **Swagger** (optional): For API documentation, testing, and easy interaction with endpoints.

## 🚀 Getting Started

### Prerequisites
- .NET SDK (version 5.0 or later)
- SQL Server, PostgreSQL, or MySQL installed

### 📦 Installation
1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/employee-management-api.git
