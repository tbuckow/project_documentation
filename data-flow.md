# Datenfluss

Beschreibt den Datenfluss im Projekt.

# Datenflussdiagramm

```mermaid
flowchart TD
    User[Benutzer]
    UI[Web-Oberfläche]
    API[Controller/API]
    Service[Service-Schicht]
    JSON[JSON-Datei: Bücher]
    XML[XML-Datei: Mitglieder]
    Flat[Flat File: Ausleihen]
    DB[SQLite Datenbank]
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

## Beschreibung
- **Benutzer** interagiert mit der Web-Oberfläche (UI).
- Die UI sendet Anfragen an die Controller/API.
- Die API ruft die Service-Schicht auf.
- Die Service-Schicht verarbeitet die Geschäftslogik und kommuniziert mit:
  - der SQLite-Datenbank (z.B. für persistente Daten)
  - JSON-Dateien (Bücher)
  - XML-Dateien (Mitglieder)
  - Flat Files (Ausleihen)
  - Logdatei (logs.txt) für Aktionen.
