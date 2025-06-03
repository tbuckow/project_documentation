# ER-Diagram

Here is the Entity-Relationship-Diagram of the project.

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

## Description
- A **Member** can borrow multiple books (BORROW), a **Book** can be borrowed multiple times.
- The **BORROW** entity links books and members with borrow and return dates.
