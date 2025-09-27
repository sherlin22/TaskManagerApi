# TaskManagerApi

A simple **Task Manager REST API** built with **ASP.NET Core Web API** and **Entity Framework Core (InMemory database)**.  
This project demonstrates how to build a clean and professional API with CRUD operations, Swagger UI, and proper project structure.

---

## 🚀 Features
- User can **Create, Read, Update, Delete (CRUD)** tasks.
- Each Task has:
  - `Id` (auto-generated)
  - `Title`
  - `Description`
  - `IsComplete` status (true/false)
- Uses **Entity Framework Core InMemory Database** (easy for testing & demo).
- Integrated **Swagger UI** for API testing.
- Built with **.NET 9** (latest SDK).

---

## 🛠️ Tech Stack
- **Backend**: ASP.NET Core Web API  
- **Database**: EF Core InMemory (will upgrade to SQLite for production)  
- **Tools**: Swagger (API documentation & testing), Visual Studio Code, Git/GitHub  

---

## 📂 Project Structure
TaskManagerApi/
│── Controllers/ → API controllers (TasksController.cs)
│── Data/ → EF Core DbContext (TaskContext.cs)
│── Models/ → Data models (TaskItem.cs)
│── Program.cs → App startup
│── appsettings.json → Configurations


---

## ▶️ Getting Started

### 1. Clone the repo

```bash
git clone https://github.com/sherlin22/TaskManagerApi.git
cd TaskManagerApi

### 2. Run the project
dotnet run

### 3. Open Swagger UI
Go to:
http://localhost:5086/swagger
API Endpoints
GET /api/tasks → Get all tasks
GET /api/tasks/{id} → Get a task by Id
POST /api/tasks → Create a new task
PUT /api/tasks/{id} → Update an existing task
DELETE /api/tasks/{id} → Delete a task