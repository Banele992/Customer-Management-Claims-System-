# 📄💼 Contract Monthly Claim System (CMCS)

**Contract Monthly Claim System (CMCS)** is a web-based application developed using **ASP.NET Core MVC**. This system is designed to **streamline the process of submitting and approving monthly claims** for **Independent Contractor (IC) lecturers**, reflecting real-world administrative workflows in academic institutions.

The system offers an intuitive and interactive interface for lecturers to manage their claims, upload supporting documentation, and track approval statuses — enhancing efficiency, accuracy, and accountability.

---
## Home Page

---![image](https://github.com/user-attachments/assets/e599e37e-b1f1-4868-a895-983c9c4c9c9a)

## 🧭 Key Objectives

* 📝 Simplify monthly claim submissions by IC lecturers
* 🔍 Enable detailed verification by Programme Coordinators and Academic Managers
* 📂 Support document uploads for claim verification
* 💰 Perform automated calculations based on hours worked and hourly rates
* 📊 Ensure administrative transparency and process accountability

---

## 📌 Key Features

* ✅ Role-based access (Lecturer, Programme Coordinator, Academic Manager)
* 🧮 Automated claim calculations based on inputted work hours and pay rates
* 📤 Upload and manage supporting documents
* 🔄 Approval workflow with audit trails
* 📅 View monthly claim history and claim status updates
* 🧾 Admin dashboard for tracking and managing all claims

---

## 🛠️ Tech Stack

* **Backend:** ASP.NET Core MVC 7
* **Frontend:** Razor Pages, Bootstrap 5
* **Database:** SQL Server with Entity Framework Core
* **Authentication:** ASP.NET Core Identity
* **File Handling:** IFormFile (for uploading documents)
* **Other:** LINQ, DataAnnotations, RESTful controllers

---

## 💻 System Requirements

To run this application, ensure the following tools and frameworks are installed:

* **.NET SDK:** .NET 7.0 or later
* **IDE:** Visual Studio 2022+ or VS Code with C# extensions
* **Database:** SQL Server (LocalDB or SQL Server Express)
* **Git:** To clone the repository

---

## 📦 Dependencies

Key NuGet packages used in this project include:

* `Microsoft.AspNetCore.Identity.EntityFrameworkCore`
* `Microsoft.EntityFrameworkCore.SqlServer`
* `Microsoft.EntityFrameworkCore.Tools`
* `Microsoft.AspNetCore.Mvc.Razor.RuntimeCompilation`
* `Microsoft.AspNetCore.Authentication.Cookies`

These packages are restored automatically during build.

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/cmcs.git
cd cmcs
```

### 2. Open the Project in Visual Studio

Open the solution file `CMCS.sln` in **Visual Studio**.

### 3. Configure the Database

Update the connection string in `appsettings.json`:

```json
"ConnectionStrings": {
  "DefaultConnection": "Server=(localdb)\\mssqllocaldb;Database=CMCSDB;Trusted_Connection=True;"
}
```

### 4. Apply Migrations & Seed the Database

Open **Package Manager Console** and run:

```bash
Update-Database
```

### 5. Run the Application

Click **Start** in Visual Studio or run in terminal:

```bash
dotnet run
```

---

## 📁 Project Structure Overview

```
CMCS/
├── Controllers/           → Application logic and claim handling
├── Models/                → Entity classes for Lecturer, Claim, etc.
├── Views/                 → Razor view files
├── Data/                  → DbContext and migrations
├── wwwroot/               → Static assets (CSS, JS, uploads)
├── appsettings.json       → Configuration settings
└── Program.cs / Startup.cs → Service registration and middleware
```

---

## 📚 Learning Goals (For Students)

By building this system, you will:

* 💡 Understand .NET GUI development in real-world scenarios
* 🛠️ Practice implementing MVC architecture with C#
* 🧑‍💻 Gain hands-on experience with Entity Framework Core
* 🔐 Apply role-based access control with ASP.NET Identity
* 🖼️ Learn to handle file uploads and data validation
* 📂 Build and deploy a robust business application

---

## 🧑‍🏫 Educational Use

This project is part of the **.NET Software Development Module**, designed to prepare students for professional development scenarios by simulating complex business logic, stakeholder interactions, and real-time data handling within web applications.
