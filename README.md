Employee Management System
A modern Spring Boot + Thymeleaf based web application that performs CRUD operations (Create, Read, Update, Delete) on Employee data. Includes features like pagination, sorting, and a clean, responsive Bootstrap 4-based UI.


📚 Key Features

| Feature                | Description                                                   
| ---------------------- | ------------------------------------------------------------- 
| ➕ **Add Employee**     | Create a new employee with name and email.                    
| ✏️ **Update Employee** | Edit existing employee details.                               
| ❌ **Delete Employee**  | Remove an employee permanently.                               
| 📋 **List View**       | View all employees with pagination and sorting on name/email. 


⚙️ Technology Stack
| Layer         | Technology                   |
| ------------- | ---------------------------- |
| 🧠 Backend    | Spring Boot, Spring Data JPA |
| 🗃️ Database  | MySQL                        |
| 🎨 Frontend   | Thymeleaf + Bootstrap        |
| 📦 Build Tool | Maven                        |
| 🧪 Testing    | JUnit 5                      |

📁 Project Structure
src/
├── main/
│   ├── java/net/javaguides/springboot/
│   │   ├── controller/         // Web controllers
│   │   ├── model/              // Employee Entity
│   │   ├── repository/         // JPA Repository
│   │   ├── service/            // Business logic
│   │   └── SpringbootThymeleafCrudWebAppApplication.java
│   └── resources/
│       ├── templates/          // Thymeleaf HTML files
│       └── application.properties

 employee-management-system

🗃️ Step 2: Configure MySQL
Open MySQL Workbench and run:



CREATE DATABASE Project;
Then update src/main/resources/application.properties:

spring.datasource.url=jdbc:mysql://localhost:3306/Project?useSSL=false
spring.datasource.username=root
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update


▶️ Step 3: Run the Application
Using Maven Wrapper:
./mvnw spring-boot:run



 Setup Instructions
🧵 Step 1: Clone the Project


🌐 Open in Browser
http://localhost:8080/




🧠 Future Enhancements
✅ Add Spring Security login/logout

📥 Export Employee list to PDF/Excel

🖼️ Add profile photo upload

🌍 Deploy to cloud (Heroku/AWS)
