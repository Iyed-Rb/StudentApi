# 📚 Student API (ASP.NET Core)

A simple **ASP.NET Core Web API** project for managing students.  
This project is a **learning exercise** to practice **REST APIs**, **layered architecture**, and **API consumption** using a client application.

The solution is divided into:  
- **Server (API)**
- **Client (Console App)**

---

## 🧩 Project Structure

### 🔹 Server Side (Web API)
Built using a **3-Tier Architecture**:

- **StudentApi** → API layer (Controllers, Program, configuration)  
- **StudentApiBusinessLayer** → Business logic  
- **StudentDataAccessLayer** → Data access (in-memory data)  

This separation keeps the code **organized** and **easy to maintain**.

### 🔹 Client Side (Console Application)
A **C# Console App** that consumes the API using `HttpClient`.  

The client can:
- Send HTTP requests to the API  
- Display results in the console  
- Demonstrate how a real client interacts with a Web API  

---

## ✨ Features
- Get all students  
- Get passed students  
- Get failed students  
- Get student by ID  
- Add a new student  
- Update an existing student  
- Delete a student  
- Calculate average grade  

---

## 🔗 API Endpoints (Server)

| Action                | Endpoint                     | Method |
|-----------------------|------------------------------|--------|
| Get all students      | `/api/students/all`          | GET    |
| Get passed students   | `/api/students/passed`       | GET    |
| Get failed students   | `/api/students/failed`       | GET    |
| Get student by ID     | `/api/students/{id}`         | GET    |
| Add student           | `/api/students`              | POST   |
| Update student        | `/api/students/{id}`         | PUT    |
| Delete student        | `/api/students/{id}`         | DELETE |
| Average grade         | `/api/students/averagegrade` | GET    |

---

## 🖥️ Client Operations
The console client demonstrates:  
- Fetching all students  
- Fetching passed students  
- Calculating the average grade  
- Finding students by ID  
- Adding a student  
- Updating a student  
- Deleting a student  

_All results are printed clearly in the console._

---

## 🛠️ Technologies Used
- C#  
- ASP.NET Core Web API  
- Console Application (Client)  
- `HttpClient`  
- Swagger (for API testing)  
- Visual Studio  

---

## ▶️ How to Run
1. Open the solution in **Visual Studio**  
2. Run the **StudentApi** project first  
3. Make sure the **API URL** matches the one used in the client  
4. Run the **StudentApiClient** project  
5. Observe the API interaction in the console  

---

## 🌱 Future Improvements
- Configure **EF Core** for database storage  
- Add more **input validation**  
- Apply additional **ASP.NET concepts** as I continue learning backend development
