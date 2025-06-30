
🎓 Student Management System using Spring Boot & Thymeleaf
🚀 Motivation
In earlier projects like Todo Management and User Management, CRUD operations were performed using Spring Boot, but the interaction required tools like Postman or writing custom JSON requests. This manual process was tedious and impractical for regular use.

This project improves usability by adding a user-friendly web interface using Thymeleaf, allowing users to interact with the system via forms and buttons, without relying on external clients or manual API calls.

🌐 Introduction to Thymeleaf
Thymeleaf is a modern server-side Java template engine for processing HTML, XML, JavaScript, and more. It integrates seamlessly with Spring MVC, making it easy to build full-featured web applications.

📌 How It Works:
Thymeleaf follows a decoupled architecture, separating view logic from application logic.

Spring Boot auto-configures Thymeleaf when it's present in the classpath.

Controller methods pass model data, which Thymeleaf templates can access through expressions like ${student.name}.

Templates are processed from the resources/templates/ folder.

🧱 Project Architecture


⚙️ Setup Instructions
🔧 Prerequisites:
Java 8 or higher

MySQL Server

Maven

IntelliJ IDEA / Eclipse

📝 Steps to Run:
Clone the repository

git clone https://github.com/Gopikakavi/Student-Management-System-using-Spring-Thymeleaf-mysql.git
Open in your IDE (IntelliJ IDEA recommended).
No need to adjust dependencies — all required libraries are included via Maven.

Configure MySQL database in application.properties:

spring.datasource.url=jdbc:mysql://localhost:3306/your_db_name
spring.datasource.username=your_username
spring.datasource.password=your_password

spring.jpa.hibernate.ddl-auto=update
spring.jpa.database-platform=org.hibernate.dialect.MySQL8Dialect
Run the application (StudentManagementApplication.java as Spring Boot app).

Visit in your browser:

http://localhost:8080/students
💻 Features
✅ View all students in a table

➕ Add new students

📝 Edit existing student details

❌ Delete students

👁️ View student information

✅ Form validations using Spring Validation annotations

🛠 Technologies Used
Layer	Technology
Backend	Java, Spring Boot, Spring Data JPA
Frontend	Thymeleaf, HTML, Bootstrap
Database	MySQL
Build Tool	Maven
