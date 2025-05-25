To-Do Application with Spring Boot and Thymeleaf
A web-based To-Do application built using Spring Boot and Thymeleaf. This application allows users to manage tasks efficiently with a clean and responsive interface.
Features

Add new tasks with a title.
View a list of all tasks.
Delete tasks.
Mark tasks as completed or pending.
Responsive design for desktop and mobile users.

Technologies Used

Spring Boot: Backend framework (version 3.x).
Thymeleaf: Template engine for rendering dynamic HTML.
Java: Version 17 or higher.
Maven: Build and dependency management.
H2 Database: In-memory database for development.
Bootstrap: For responsive front-end styling.
Spring Data JPA: For database operations.

Prerequisites
To run this application, ensure you have:

Java JDK: Version 17 or higher.
Maven: Version 3.6.0 or higher.
Git: For cloning the repository.
(Optional) An IDE like IntelliJ IDEA, Eclipse, or VS Code.

Setup Instructions

Clone the Repository:
git clone https://github.com/prathameshkaratkar/Task-Tracker-Spring-Boot.git
cd Task-Tracker-Spring-Boot


Configure the Database:

By default, the application uses an H2 in-memory database, requiring no setup.
To use a different database (e.g., MySQL), modify src/main/resources/application.properties:spring.datasource.url=jdbc:mysql://localhost:3306/todo_db
spring.datasource.username=your_username
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQLDialect




Build the Project:
mvn clean install


Run the Application:
mvn spring-boot:run

Alternatively, run the main class TodoApplication from your IDE.

Access the Application:

Navigate to http://localhost:8080 in a web browser.
The To-Do application’s homepage will load.



Usage

Add a Task: Click "Add Task," enter the title and description, and save.
View Tasks: All tasks are displayed on the homepage with their status.
Edit a Task: Click "Edit" next to a task to update its details.
Delete a Task: Click "Delete" to remove a task.
Mark as Completed: Use the toggle to mark tasks as completed or pending.

Project Structure
todo-app/
├── src/
│   ├── main/
│   │   ├── java/com/example/todo/
│   │   │   ├── controller/     # Handles HTTP requests
│   │   │   ├── model/         # Task entity and data models
│   │   │   ├── repository/    # JPA repositories for database access
│   │   │   ├── service/       # Business logic and service layer
│   │   ├── resources/
│   │   │   ├── templates/     # Thymeleaf HTML templates
│   │   │   ├── static/        # CSS, JavaScript, and Bootstrap files
│   │   │   ├── application.properties  # Application configuration
├── pom.xml                    # Maven dependencies
├── README.md                  # This file

Contributing
Contributions are welcome! To contribute:

Fork the repository.
Create a feature branch (git checkout -b feature/your-feature).
Commit your changes (git commit -m "Add your feature").
Push to the branch (git push origin feature/your-feature).
Open a pull request.


