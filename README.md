# Library Management System

A web-based library management system built with **ASP.NET Core MVC**, **Entity Framework Core**, and **SQLite**.

## Project Overview

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

## Evidence of GitHub Copilot Usage

- Numerous prompts were used during development, e.g.:
  - "Build a web-based library management system using ASP.NET Core MVC and Entity Framework Core with SQLite."
  - "Implement logging for all lend and return actions to logs.txt."
  - "Write modular xUnit test classes for BookService, MemberService, BorrowService, DataSeeder, and integration tests."
- Copilot was used for code completion, architecture suggestions, and documentation drafts.
- Evidence of Copilot usage can be found in commit messages and the project structure.

## Reflection: Copilot Experience

GitHub Copilot significantly accelerated development by suggesting boilerplate code, test cases, and documentation templates. Copilot was especially helpful in structuring services and creating sample APIs. Challenges arose with more complex logic and adapting generated code to project-specific requirements, which required manual adjustments. Overall, Copilot increased productivity and improved code quality by suggesting best practices.

## Testing

- Modular xUnit tests
- Test data isolation
- Sequential execution to avoid file conflicts

For more details, see:

- [`architecture.md`](architecture.md)
- [`er-diagram.md`](er-diagram.md)
- [`api-docs.md`](api-docs.md)
- [`setup.md`](setup.md)
- [`CONTRIBUTING.md`](CONTRIBUTING.md)
