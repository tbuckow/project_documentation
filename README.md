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

## Evidence of GitHub Copilot Usage

- Während der Entwicklung wurden zahlreiche Prompts an Copilot gestellt, z.B.:
  - "Build a web-based library management system using ASP.NET Core MVC and Entity Framework Core with SQLite."
  - "Implement logging for all lend and return actions to logs.txt."
  - "Write modular xUnit test classes for BookService, MemberService, BorrowService, DataSeeder, and integration tests."
- Copilot wurde für Code-Vervollständigungen, Architekturvorschläge und Dokumentationsentwürfe genutzt.
- Hinweise auf Copilot-Nutzung sind in den Commit-Nachrichten und der Projektstruktur dokumentiert.

## Reflection: Copilot Experience

GitHub Copilot hat die Entwicklung deutlich beschleunigt, indem es Boilerplate-Code, Testfälle und Dokumentationsvorlagen vorgeschlagen hat. Besonders hilfreich war Copilot bei der Strukturierung von Services und beim Erstellen von Beispiel-APIs. Herausforderungen gab es bei komplexeren Logiken und der Anpassung von generiertem Code an projektspezifische Anforderungen – hier war manuelles Nacharbeiten nötig. Insgesamt hat Copilot die Produktivität gesteigert und die Codequalität durch Vorschläge zu Best Practices verbessert.

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
