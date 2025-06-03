# Library Management System

A web-based library management system built with **ASP.NET Core MVC**, **Entity Framework Core**, and **SQLite**.

##  Project Overview

This application allows you to manage books, members, and lending operations for a library. Data is stored in JSON, XML, and flat files.

### Purpose

To provide a lightweight, file-based library management system for small institutions or personal use.

### Key Features

- **Book Management**: Add, search, and list books
- **Member Management**: Register and list members
- **Lending System**: Lend and return books, view lending history
- **Data Storage**:
  - Books: JSON
  - Members: XML
  - Borrow Records: Flat file
- **Logging**: All lending/return actions are logged to `Data/logs.txt`

### Technology Stack

- ASP.NET Core MVC
- Entity Framework Core
- SQLite
- JSON, XML, Flat Files
- xUnit for testing

### Target Users

- Small libraries
- Schools or universities
- Developers learning clean architecture and file-based data handling

##  Copilot Usage

This project was developed with GitHub Copilot assistance. Prompts included:

- "Build a web-based library management system using ASP.NET Core MVC and Entity Framework Core with SQLite."
- "Implement logging for all lend and return actions to logs.txt."
- "Write modular xUnit test classes for BookService, MemberService, BorrowService, DataSeeder, and integration tests."

##  Testing

- Modular xUnit tests
- Test data isolation
- Sequential execution to avoid file conflicts


 For more details, see:

- [`architecture.md`](architectured`
- `er-diagram.md`
- `api-docs.md`
- `setup.md`
- `CONTRIBUTING.md`
