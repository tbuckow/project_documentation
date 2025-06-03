# Data Flow

Describes the data flow in the project.

# Data Flow Diagram

```mermaid
flowchart TD
    User[User]
    UI[Web UI]
    API[Controller/API]
    Service[Service Layer]
    JSON[JSON File: Books]
    XML[XML File: Members]
    Flat[Flat File: Borrow Records]
    DB[SQLite Database]
    Log[logs.txt]

    User --> UI
    UI --> API
    API --> Service
    Service --> DB
    Service --> JSON
    Service --> XML
    Service --> Flat
    Service --> Log
```

## Description
- **User** interacts with the web UI.
- The UI sends requests to the controllers/API.
- The API calls the service layer.
- The service layer processes business logic and communicates with:
  - the SQLite database (for persistent data)
  - JSON files (books)
  - XML files (members)
  - flat files (borrow records)
  - log file (logs.txt) for actions.
