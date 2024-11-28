
# 😂 Meme App - A Fun CRUD Project with .NET C# and SQL Server 🎉

Welcome to **Jokes App**, a delightful application where you can **Create**, **Read**, **Update**, and **Delete** jokes. Built with the power of `.NET C#` and **SQL Server**, this app will tickle your funny bone while showcasing clean and efficient CRUD operations.  

---

## 📋 Table of Contents
1. [📖 About](#-about)
2. [🚀 Features](#-features)
3. [🛠 Prerequisites](#-prerequisites)
4. [📥 Installation Guide](#-installation-guide)
5. [🏃 Running Guide](#-running-guide)
6. [🛢 SQL Server Configuration](#-sql-server-configuration)
7. [📌 API Endpoints](#-api-endpoints)
8. [📸 Screenshots](#-screenshots)
9. [💡 Jokes API Example](#-jokes-api-example)
10. [📜 License](#-license)

---

## 📖 About
The **Jokes App** is a CRUD-based project where users can manage jokes through a seamless UI. The backend is powered by `.NET C#`, while SQL Server handles data storage. Perfect for learning or showcasing **CRUD operations** with a sprinkle of humor!

---

## 🚀 Features
✅ Add your favorite jokes  
✅ View all jokes with pagination  
✅ Edit existing jokes  
✅ Delete jokes you no longer find funny  

---

## 🛠 Prerequisites
Before you begin, ensure you have the following tools installed:

| **Tool**            | **Version**                  |
|---------------------|------------------------------|
| Visual Studio       | 2022 or later               |
| .NET SDK            | 6.0 or later                |
| SQL Server          | 2019 or later               |
| Entity Framework    | Core 6.0                    |

---

## 📥 Installation Guide
1. Clone the repository:  
   ```bash
   git clone https://github.com/your-username/jokes-app.git
   cd jokes-app
   ```

2. Open the project in **Visual Studio**.

3. Restore NuGet packages:  
   ```bash
   dotnet restore
   ```

4. Update the **appsettings.json** file with your SQL Server connection string:
   ```json
   "ConnectionStrings": {
     "DefaultConnection": "Server=YOUR_SERVER_NAME;Database=JokesDB;Trusted_Connection=True;MultipleActiveResultSets=true"
   }
   ```

5. Run database migrations:  
   ```bash
   dotnet ef database update
   ```

---

## 🏃 Running Guide
1. Open the project in **Visual Studio**.
2. Set the startup project to **JokesApp.API**.
3. Press `F5` or run the project using the play button ▶️.
4. Access the app at:  
   **Frontend:** `http://localhost:5000`  
   **API:** `http://localhost:5000/api/jokes`

---

## 🛢 SQL Server Configuration
### Step 1: Create the Database
1. Open **SQL Server Management Studio** (SSMS).
2. Create a new database called `JokesDB`:
   ```sql
   CREATE DATABASE JokesDB;
   ```

### Step 2: Update Connection String
Update your **appsettings.json** file with your SQL Server name:
```json
"ConnectionStrings": {
  "DefaultConnection": "Server=YOUR_SERVER_NAME;Database=JokesDB;Trusted_Connection=True;"
}
```

### Step 3: Run Migrations
In the terminal, execute:
```bash
dotnet ef migrations add InitialCreate
dotnet ef database update
```

---

## 📌 API Endpoints
| **Method** | **Endpoint**        | **Description**                  |
|------------|---------------------|----------------------------------|
| `GET`      | `/api/jokes`        | Fetch all jokes                 |
| `POST`     | `/api/jokes`        | Add a new joke                  |
| `PUT`      | `/api/jokes/{id}`   | Update an existing joke         |
| `DELETE`   | `/api/jokes/{id}`   | Delete a joke                   |

---

## 📸 Screenshots
Coming soon! 🎨

---

## 💡 Jokes API Example
Here’s a quick joke for you:
```json
{
  "id": 1,
  "content": "Why don’t skeletons fight each other? They don’t have the guts!"
}
```

---

## 📜 License
This project is licensed under the MIT License.  
Feel free to use, modify, and share!

---

✨ *Happy coding! Keep joking!* 🎉 - Nuu
