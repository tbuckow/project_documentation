# Architektur

```mermaid
graph TD
    A[Frontend (ASP.NET Core MVC)]
    B[Backend (Controllers, Services, Logging)]
    C[Entity Framework Core]
    D[SQLite Database]
    E[JSON File Storage]
    F[XML File Storage]
    G[Flat File Storage]
    H[Logs (logs.txt)]

    A --> B
    B --> C
    C --> D
    B --> E
    B --> F
    B --> G
    B --> H
```

## Komponentenbeschreibung

- **Frontend**: Benutzeroberfläche mit ASP.NET Core MVC
- **Backend**: Geschäftslogik, Controller, Services, Logging
- **Entity Framework Core**: ORM für Datenbankzugriffe
- **SQLite**: Relationale Datenbank für persistente Speicherung
- **JSON, XML, Flat Files**: Dateibasierte Speicherung für verschiedene Entitäten
- **Logs**: Protokollierung aller Ausleih- und Rückgabeaktionen
