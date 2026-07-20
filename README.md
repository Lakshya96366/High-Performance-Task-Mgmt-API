# ☁️ Cloud-Native Task Management API

A high-performance, scalable RESTful API built with **FastAPI** and **SQLAlchemy**. This project demonstrates modern backend architecture principles, including strict data validation, efficient database session management, and modular design ready for containerization.

## 🚀 Features
- **Robust CRUD Operations**: Create, read, update, and delete tasks with strict data integrity.
- **Data Validation**: Utilizes **Pydantic** schemas to ensure incoming and outgoing data strictly conforms to expected formats.
- **Optimized Resource Management**: Implements FastAPI’s dependency injection system (`Depends`) for safe, leak-proof database session handling.
- **Scalability Ready**: Features built-in pagination and comprehensive HTTP error handling, establishing a foundation ready for Docker containerization and cloud deployment.

## 🛠️ Tech Stack
- **Language**: Python
- **Framework**: FastAPI
- **Database ORM**: SQLAlchemy
- **Validation**: Pydantic
- **Database**: SQLite (easily swappable for PostgreSQL/MySQL)

## 📡 API Endpoints

| Method | Endpoint | Description |
| :--- | :--- | :--- |
| `POST` | `/tasks/` | Create a new task |
| `GET` | `/tasks/` | Retrieve all tasks (supports `skip` and `limit` for pagination) |
| `PUT` | `/tasks/{task_id}` | Update an existing task by ID |
| `DELETE` | `/tasks/{task_id}` | Delete a task by ID |

*Note: Interactive API documentation is automatically generated and available at `/docs` (Swagger UI) and `/redoc` when the server is running.*


