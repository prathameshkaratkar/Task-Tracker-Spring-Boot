Here is a complete `README.md` file based on your description:

````markdown
# To-Do Application with Spring Boot and Thymeleaf

A web-based To-Do application built using Spring Boot and Thymeleaf. This application allows users to manage tasks efficiently with a clean and responsive interface.

---

## ✨ Features

- ✅ Add new tasks with a title and description.
- 📋 View a list of all tasks.
- ❌ Delete tasks.
- 🔄 Mark tasks as completed or pending.
- 📱 Responsive design for desktop and mobile users.

---

## 🛠 Technologies Used

- **Spring Boot**: Backend framework (version 3.x)
- **Thymeleaf**: Template engine for rendering dynamic HTML
- **Java**: Version 17 or higher
- **Maven**: Build and dependency management
- **H2 Database**: In-memory database for development
- **Bootstrap**: For responsive front-end styling
- **Spring Data JPA**: For database operations

---

## ✅ Prerequisites

To run this application, ensure you have:

- Java JDK: Version 17 or higher
- Maven: Version 3.6.0 or higher
- Git: For cloning the repository
- (Optional) An IDE like IntelliJ IDEA, Eclipse, or VS Code

---

## 🚀 Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/prathameshkaratkar/Task-Tracker-Spring-Boot.git
cd todo-app
````

### 2. Configure the Database

By default, the application uses an **H2 in-memory database** — no setup required.

To use a different database (e.g., MySQL), modify:
`src/main/resources/application.properties`

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/todo_app
spring.datasource.username=your_username
spring.datasource.password=your_password
spring.jpa.hibernate.ddl-auto=update
spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQLDialect
```

### 3. Build the Project

```bash
mvn clean install
```

### 4. Run the Application

```bash
mvn spring-boot:run
```

Alternatively, run the `TodoApplication` class from your IDE.

---

## 🌐 Access the Application

Open your browser and navigate to:
[http://localhost:8080](http://localhost:8080)

---

## 📋 Usage

* **Add a Task**: Click **"Add Task"**, enter the title and description, then save.
* **View Tasks**: All tasks are shown on the homepage with their status.
* **Edit a Task**: Click **"Edit"** next to a task to update its details.
* **Delete a Task**: Click **"Delete"** to remove a task.
* **Mark as Completed**: Use the checkbox or toggle to change the task status.

---

## 📁 Project Structure

```
todo-app/
├── src/
│   ├── main/
│   │   ├── java/com/example/todo/
│   │   │   ├── controller/       # Handles HTTP requests
│   │   │   ├── model/            # Task entity and data models
│   │   │   ├── repository/       # JPA repositories for database access
│   │   │   ├── service/          # Business logic and service layer
│   ├── resources/
│   │   ├── templates/            # Thymeleaf HTML templates
│   │   ├── static/               # CSS, JavaScript, and Bootstrap files
│   │   ├── application.properties  # Application configuration
├── pom.xml                       # Maven dependencies
├── README.md                     # This file
```

---

## 🤝 Contributing

Contributions are welcome! To contribute:

1. Fork the repository.
2. Create a feature branch:

   ```bash
   git checkout -b feature/your-feature
   ```
3. Commit your changes:

   ```bash
   git commit -m "Add your feature"
   ```
4. Push to the branch:

   ```bash
   git push origin feature/your-feature
   ```
5. Open a pull request.

Please include tests and follow the project’s coding standards.

---

