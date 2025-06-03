# ER-Diagramm

Hier befindet sich das Entity-Relationship-Diagramm des Projekts.

# Entity Relationship Diagram (ERD)

```mermaid
erDiagram
    BOOK ||--o{ BORROW : lends
    MEMBER ||--o{ BORROW : borrows
    BOOK {
        int Id
        string Title
        string Author
        string ISBN
        int Year
    }
    MEMBER {
        int Id
        string Name
        string Email
        string Address
    }
    BORROW {
        int Id
        date BorrowDate
        date ReturnDate
        int BookId
        int MemberId
    }
```

## Beschreibung
- Ein **Member** kann mehrere Bücher ausleihen (BORROW), ein **Book** kann mehrfach ausgeliehen werden.
- Die Entität **BORROW** verbindet Bücher und Mitglieder mit Ausleih- und Rückgabedatum.
