# Backend: .NET Core

---

## Getting Started

Before you begin, ensure you have the following installed on your machine:

- [.NET SDK](https://dotnet.microsoft.com/download) (version X.X or higher)
- [MySQL](https://dev.mysql.com/downloads/installer/) (or a compatible SQL database)
- [Visual Studio](https://visualstudio.microsoft.com/) or [VSCode](https://code.visualstudio.com/)

---

## Installation

1. **Clone the repository:**
   ```bash
   $ git clone https://github.com/your-username/your-repo.git
2. **Navigate to the project folder:**
   ```bash  
   $ cd your-project-folder

3. **Install dependencies: Restore the required .NET packages by running the following command:**
   ```bash
   $ dotnet restore
4. **Configure the database: Make sure MySQL is running. Create a new database and update the connection string in appsettings.json to reflect your MySQL credentials:**
    ```bash
   "ConnectionStrings": {
   "DefaultConnection": "Server=localhost;Database=your_database_name;User=root;Password=your_password;"}
 ## Database Migrations: To apply the database migrations and create the necessary tables, run the following command:
    ```bash
    $ dotnet ef database update
 ## Running the Project: Once the database is set up and dependencies are installed, you can run the project with:
    ```bash
    $ dotnet run
By default, the application will be accessible at https://localhost:5001 (or http://localhost:5000).

 ##  **API Documentation**
This project includes RESTful APIs for performing CRUD operations. You can use Postman or similar tools to interact with the APIs. API documentation is available at /swagger when the application is running.
##  **MySQL Integration**
The project uses MySQL for persistent data storage. Entity Framework Core is used as the Object-Relational Mapping (ORM) tool to interact with the database. CRUD operations for entities such as "Student" are handled through services and repositories, ensuring a clean and modular architecture.
