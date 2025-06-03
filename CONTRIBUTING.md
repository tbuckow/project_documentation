# Beitragende

## Wie du beitragen kannst

1. **Forke das Repository**
2. **Erstelle einen neuen Branch** für deine Änderung:
   ```powershell
   git checkout -b feature/dein-feature-name
   ```
3. **Nimm deine Änderungen vor**
4. **Committe deine Änderungen**:
   ```powershell
   git add .
   git commit -m "Beschreibe deine Änderung"
   ```
5. **Pushe den Branch zu deinem Fork**:
   ```powershell
   git push origin feature/dein-feature-name
   ```
6. **Erstelle einen Pull Request** auf GitHub gegen den `main`-Branch

## GitHub Workflow Tipps

- Nutze beschreibende Branch-Namen (z.B. `feature/login`, `bugfix/validation-error`)
- Schreibe klare und prägnante Commit-Nachrichten
- Führe vor dem PR alle Tests lokal aus (`dotnet test`)
- Halte deinen Branch aktuell mit `main` (z.B. durch `git merge main`)
- Beschreibe im Pull Request, was du geändert hast und warum
- Kleine, thematisch fokussierte Pull Requests sind leichter zu reviewen

## Code Style

- Halte dich an die bestehenden Coding-Guidelines und Formatierungen
- Dokumentiere neue oder geänderte Funktionen ausreichend

## Hinweise

- Respektiere die Code of Conduct und die Community-Richtlinien
- Bei Fragen oder Problemen: Erstelle ein Issue oder diskutiere im Pull Request
