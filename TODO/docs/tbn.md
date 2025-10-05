# Rules & Guidelines for Implementation

## General Coding Rules
- Use **camelCase** for variables, methods, and properties.
- Follow **MVC (Model–View–Controller)** architecture.
- Maintain proper **package structure** (e.g., `model/`, `controller/`, `service/`, `repository/`).

## Framework & Tools
- **Spring Boot** (latest stable version).
- **Maven** for dependency management and builds.
- Use **RESTful APIs** for communication (JSON input/output).

## Data Storage
- Store todos in a **JSON file** for now.
- The JSON file should persist data across server restarts.
- Keep storage logic modular so it can be swapped with a real DB in the future.

## API Endpoints (Draft)
1. `POST /todos` → create a new todo (for current date only).  
2. `GET /todos` → fetch all todos from the past 7 days.  
3. `DELETE /todos/{id}` → delete a todo by ID.  

---
