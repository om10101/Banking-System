# 🏦 Banking Management System

A desktop-based **Banking Management System** built using **Java Swing, JDBC, and MySQL**. The application provides a graphical interface for managing banking operations, including user login, account management, deposits, withdrawals, and transaction processing.

The project demonstrates Java GUI development, database connectivity, SQL operations, and event-driven programming.

## ✨ Features

- 🔐 **User Authentication** — Login interface for accessing banking operations.
- 👤 **Account Management** — Manage customer banking details.
- 💰 **Deposit Money** — Deposit money into an account.
- 💸 **Withdraw Money** — Withdraw money based on the available balance.
- 📊 **Balance Enquiry** — Check the current account balance.
- 📜 **Transaction Handling** — Perform banking transactions through database operations.
- 🖥️ **Graphical User Interface** — Interactive desktop interface built with Java Swing.
- 🗄️ **Database Integration** — Store and retrieve banking data using MySQL and JDBC.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Java | Core application logic |
| Java Swing & AWT | Desktop graphical user interface |
| JDBC | Java-to-database connectivity |
| MySQL | Database management |
| IntelliJ IDEA / Eclipse | Development environment |

## 🏗️ Application Architecture

The application follows a simple desktop application architecture:

```text
Banking-System
│
├── Java Swing UI
│   ├── Login
│   ├── Signup / Account Creation
│   ├── Deposit
│   ├── Withdrawal
│   └── Balance Enquiry
│
├── Application Logic
│   ├── Event Handling
│   ├── Input Validation
│   └── Banking Operations
│
└── Database Layer
    ├── JDBC Connection
    ├── SQL Queries
    └── MySQL Database
```

*Note: The diagram describes the intended application flow; adjust the modules to match your actual implementation.*

## ⚙️ Prerequisites

Before running the application, install:

- Java JDK 8 or later
- MySQL Server
- IntelliJ IDEA, Eclipse, or another Java IDE
- MySQL Connector/J JDBC driver

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/om10101/Banking-System.git
```

Navigate to the project directory:

```bash
cd Banking-System
```

### 2. Configure MySQL

Start your MySQL server and create the database:

```sql
CREATE DATABASE banksystem;
USE banksystem;
```

Create the tables required by your application before running it.

**Important:** The table names and columns must match the SQL queries in your Java source code. For example, if the login module queries a `login` table, that table must exist with the expected columns.

### 3. Configure the database connection

Locate your JDBC connection code and configure it with your local MySQL credentials.

Example:

```java
String url = "jdbc:mysql://localhost:3306/banksystem";
String username = "root";
String password = "your_mysql_password";

Connection connection = DriverManager.getConnection(
    url, username, password
);
```

Replace `your_mysql_password` with your local MySQL password.

Make sure the MySQL Connector/J driver is available in your project classpath.

### 4. Run the application

1. Open the project in IntelliJ IDEA or Eclipse.
2. Configure the JDK and MySQL JDBC driver.
3. Start MySQL Server.
4. Verify that the `banksystem` database and required tables exist.
5. Run the application's main class or login screen.
6. Create an account or log in using valid credentials, depending on the implemented workflow.

## 🔄 Application Workflow

1. The user opens the banking application.
2. The login or account creation screen appears.
3. The user accesses the available banking operations.
4. The selected operation is processed by the Java application.
5. JDBC executes the required SQL queries against MySQL.
6. The application displays the result to the user.

## 🔒 Security Considerations

This project is intended for learning and demonstration purposes. For a production-ready banking application, consider implementing:

- Password hashing instead of storing plain-text passwords.
- Prepared statements for database queries.
- Input validation and exception handling.
- Database transactions for balance updates.
- Atomic balance updates to prevent inconsistent transactions.
- Role-based access control and secure credential management.
- Transaction history and audit logging.

**Disclaimer:** This is an educational project, not a real banking system. Do not use it to manage real customer funds or sensitive financial information.

## 🎯 Learning Outcomes

Through this project, I explored:

- Java object-oriented programming.
- GUI development using Swing and AWT.
- Event handling in desktop applications.
- JDBC connectivity with MySQL.
- SQL queries and database operations.
- Implementation of common banking workflows.
- Debugging and handling database-related errors.

## 🔮 Future Enhancements

- [ ] Add secure password hashing.
- [ ] Improve database schema and validation.
- [ ] Add transaction history with timestamps.
- [ ] Implement atomic deposits and withdrawals.
- [ ] Add account statements and receipt generation.
- [ ] Improve UI design and user experience.
- [ ] Add automated tests.
- [ ] Package the application as an executable JAR.

## 👨‍💻 Author

Om Umale

- GitHub: [@om10101](https://github.com/om10101)
- LinkedIn: [om-u120604](https://www.linkedin.com/in/om-u120604/)

---

⭐ If you find this project useful for learning Java desktop development, feel free to star the repository.
