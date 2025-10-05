# Todo App – Backend PRD

## Problem Statement
We need a simple **Todo backend** that allows users to:
- Add a new todo task (restricted to the current date).
- Retrieve todos from the **past 7 days**.
- Delete a specific todo task.

This backend should be extendable so that future features can be added easily.

---

## Functional Requirements
1. **Create Todo**
   - A user can create a todo task for the **current date only**.
   - Each todo should have:
     - `id` (unique identifier)
     - `title` (string, required)
     - `description` (string, optional)
     - `dateCreated` (auto-generated, current date)
   
2. **Get Todos**
   - A user can fetch all todos from the **past 7 days (including today)**.
   - Should return todos in **reverse chronological order**.

3. **Delete Todo**
   - A user can delete a todo by `id`.

---

## Non-Functional Requirements
- Code must follow a **clean, modular structure** for easy future extension.
- API responses should be consistent and in **JSON** format.
- Lightweight persistence using a **JSON file** (instead of a full database).
- Must be easy to migrate later to a real database (e.g., MySQL, Postgres).

---
