# Week 2 — Library API Contract

```yaml
openapi: 3.0.3
paths:
  /books/{id}/borrow:
    post:
      summary: Borrow an available book
      parameters:
        - in: path
          name: id
          required: true
          schema: { type: integer }
      responses:
        '201': { description: Loan created }
        '404': { description: Book not found }
        '409': { description: Book is unavailable }
```

**Acceptance criterion:** Given an available book, when a signed-in student borrows it, then the system creates exactly one loan record.
