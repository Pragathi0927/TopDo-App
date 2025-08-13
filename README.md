# 📝 Todo Management Application

A simple **Spring Boot** web application to manage daily tasks with CRUD (Create, Read, Update, Delete) operations.  
This project demonstrates a **backend-focused Java application** using Spring Boot, Spring MVC, Spring Data JPA, and MySQL.

---

## 🚀 Features

- ✅ Add new tasks
- 📋 View all tasks  
- ✏️ Update existing tasks
- 🗑️ Delete tasks
- 💾 Persistent storage with MySQL
- 🏗️ MVC architecture with clean separation of concerns

---

## 🛠️ Tech Stack

- **Backend:** Spring Boot, Spring MVC, Spring Data JPA
- **Database:** MySQL
- **View Layer:** JSP, HTML, CSS
- **Build Tool:** Maven
- **Java Version:** 17 (or compatible)
- **Server:** Embedded Tomcat (Spring Boot default)

---

## 📂 Project Structure

```
Todo Application/
│
├── src/main/java/com/example/todo/     # Java source code
│   ├── controller/                     # Handles HTTP requests
│   ├── model/                         # Entity classes (Task, etc.)
│   ├── repository/                    # JPA repositories
│   ├── service/                       # Business logic
│   └── TodoApplication.java           # Main application entry point
│
├── src/main/resources/
│   ├── static/                        # CSS, JS, images
│   ├── templates/                     # JSP files
│   └── application.properties         # App configuration
│
├── pom.xml                            # Maven dependencies
└── README.md
```

---

## ⚙️ Setup & Installation

### 1️⃣ Clone the repository
```bash
git clone https://github.com/Pragathi0927/TopDo-App
cd todo-application
```

### 2️⃣ Configure the database
Create a MySQL database, e.g., `todo_db`

Update the `application.properties` file:
```properties
spring.datasource.url=jdbc:mysql://localhost:3306/todo_db
spring.datasource.username=your_mysql_username
spring.datasource.password=your_mysql_password
spring.jpa.hibernate.ddl-auto=update
spring.jpa.database-platform=org.hibernate.dialect.MySQLDialect
```

### 3️⃣ Build & Run the application
```bash
mvn clean install
mvn spring-boot:run
```

### 4️⃣ Access the application
Open a browser and go to:
```
http://localhost:8080
```

---

## 🗃️ Database Schema

The application uses a simple Task entity with the following structure:

| Field | Type | Description |
|-------|------|-------------|
| id | Long | Primary key (auto-generated) |
| title | String | Task title |
| description | String | Task description |
| completed | Boolean | Task completion status |
| createdDate | LocalDateTime | Task creation timestamp |

---

## 🔧 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/` | View all tasks |
| GET | `/add` | Show add task form |
| POST | `/save` | Save new task |
| GET | `/edit/{id}` | Show edit task form |
| POST | `/update` | Update existing task |
| GET | `/delete/{id}` | Delete task |

---

## 📸 Screenshots

<!-- Add screenshots of your UI here for better presentation -->
*Screenshots will be added here showing:*
- Task listing page
- Add new task form
- Edit task form
- Task completion functionality

---

## 🔄 How to Use

1. **View Tasks:** Navigate to the home page to see all your tasks
2. **Add Task:** Click "Add New Task" and fill in the details
3. **Edit Task:** Click the "Edit" button next to any task to modify it
4. **Delete Task:** Click the "Delete" button to remove a task
5. **Mark Complete:** Toggle task completion status

---

## 📌 Future Enhancements

- 🔐 User authentication & login system
- 🏷️ Task categorization & priorities
- ⏰ Due date reminders
- 📱 Responsive front-end using Bootstrap
- 🔍 Search and filter functionality
- 📊 Task analytics and reports
- 🌙 Dark mode support

---

## 🧪 Testing

To run tests:
```bash
mvn test
```

---

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/new-feature`)
3. Commit your changes (`git commit -am 'Add new feature'`)
4. Push to the branch (`git push origin feature/new-feature`)
5. Create a Pull Request

---

## 📋 Prerequisites

- Java 17 or higher
- Maven 3.6 or higher
- MySQL 8.0 or higher
- IDE (IntelliJ IDEA, Eclipse, or VS Code)

---

## 🐛 Troubleshooting

**Common Issues:**

1. **Database Connection Error:**
   - Ensure MySQL is running
   - Verify database credentials in `application.properties`
   - Check if the database exists

2. **Port Already in Use:**
   - Change server port in `application.properties`: `server.port=8081`

3. **Maven Build Fails:**
   - Ensure Java 17 is installed and configured
   - Run `mvn clean` before `mvn install`

---

## 👨‍💻 Author

**Pragathi .S**
- 📧 Email: spragathi927@gmail.com
- 🔗 GitHub: [@Pragathi0927](https://github.com/Pragathi0927/)
- 💼 LinkedIn: [pragathi0927](www.linkedin.com/in/pragathi0927)

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## ⭐ Show your support

Give a ⭐️ if this project helped you!

---

## 📞 Support

If you have any questions or need help, feel free to:
- Open an issue on GitHub
- Send me an email
- Connect with me on LinkedIn

---

*Made with ❤️ using Spring Boot*