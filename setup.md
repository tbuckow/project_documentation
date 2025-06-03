# Setup

## Voraussetzungen

- .NET 8 SDK oder höher
- Git
- Optional: Visual Studio 2022 oder Visual Studio Code

## Schritt-für-Schritt-Anleitung

1. **Repository klonen**
   ```powershell
   git clone <REPO-URL>
   cd projectDocumentation
   ```
2. **Abhängigkeiten wiederherstellen**
   ```powershell
   dotnet restore
   ```
3. **Datenbank migrieren (falls erforderlich)**
   ```powershell
   dotnet ef database update
   ```
4. **Projekt bauen**
   ```powershell
   dotnet build
   ```
5. **Projekt starten**
   ```powershell
   dotnet run
   ```
6. **Tests ausführen**
   ```powershell
   dotnet test
   ```

## Umgebungsvariablen (Beispiel)

Falls benötigt, können folgende Umgebungsvariablen gesetzt werden (z.B. in einer `.env`-Datei oder in den Projekteinstellungen):

- `ConnectionStrings__DefaultConnection` – Verbindungszeichenfolge für SQLite
- `ASPNETCORE_ENVIRONMENT` – z.B. `Development` oder `Production`

## Hinweise

- Die Daten werden in JSON-, XML- und Flat Files im `Data`-Verzeichnis gespeichert.
- Logdateien befinden sich in `Data/logs.txt`.
- Beispiel-Daten können über ein Seed-Skript oder beim ersten Start generiert werden.
