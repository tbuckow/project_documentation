# API Documentation

## Example 1: Create Book

- **Endpoint:** `/api/books`
- **Method:** POST
- **Request Format (JSON):**
  ```json
  {
    "title": "Clean Code",
    "author": "Robert C. Martin",
    "isbn": "9780132350884",
    "year": 2008
  }
  ```
- **Response Format (JSON):**
  ```json
  {
    "id": 1,
    "title": "Clean Code",
    "author": "Robert C. Martin",
    "isbn": "9780132350884",
    "year": 2008
  }
  ```

---

## Example 2: Register Member

- **Endpoint:** `/api/members`
- **Method:** POST
- **Request Format (JSON):**
  ```json
  {
    "name": "Max Mustermann",
    "email": "max@example.com",
    "address": "Musterstraße 1, 12345 Musterstadt"
  }
  ```
- **Response Format (JSON):**
  ```json
  {
    "id": 1,
    "name": "Max Mustermann",
    "email": "max@example.com",
    "address": "Musterstraße 1, 12345 Musterstadt"
  }
  ```

---

## Example 3: Borrow Book

- **Endpoint:** `/api/borrow`
- **Method:** POST
- **Request Format (JSON):**
  ```json
  {
    "bookId": 1,
    "memberId": 1,
    "borrowDate": "2025-06-03"
  }
  ```
- **Response Format (JSON):**
  ```json
  {
    "id": 1,
    "bookId": 1,
    "memberId": 1,
    "borrowDate": "2025-06-03",
    "returnDate": null
  }
  ```
