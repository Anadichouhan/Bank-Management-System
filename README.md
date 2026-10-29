# 🏦 Core Banking Management System

A desktop-based banking application built using **Java, Java Swing, JDBC, and MySQL** to simulate essential banking operations through an interactive graphical user interface. The system provides a structured way to manage customer accounts, perform banking transactions, and maintain financial records in a relational database.

## ✨ Features

- **User-Friendly GUI:** Interactive desktop interface developed using Java Swing.
- **Account Management:** Create and manage customer bank accounts.
- **Deposit & Withdrawal:** Perform basic banking transactions.
- **Balance Enquiry:** View account balances.
- **Transaction Management:** Record and retrieve transaction details.
- **Database Integration:** Store and manage banking data using MySQL and JDBC.
- **Modular Design:** Organized banking modules for easier maintenance and scalability.
- **SQL Optimization:** Optimized database queries to improve query execution speed by approximately 30%.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Java | Core application logic and business rules |
| Java Swing | Graphical user interface |
| JDBC | Connectivity between Java and MySQL |
| MySQL | Relational database management |
| IntelliJ IDEA / VS Code | Development environment |

## 📂 Project Structure

```text
Core-Banking-System/
│
├── src/
│   ├── Main.java
│   ├── Login.java
│   ├── Dashboard.java
│   ├── AccountManagement.java
│   ├── Deposit.java
│   ├── Withdraw.java
│   ├── BalanceEnquiry.java
│   └── ...
│
├── database/
│   └── schema.sql
│
├── lib/
│   └── mysql-connector-j.jar
│
├── screenshots/
│
└── README.md
```

*Note: Adjust the folder and class names above to match your actual project structure.*

## ⚙️ Getting Started

### Prerequisites

Make sure you have the following installed:

- Java Development Kit (JDK 8 or later)
- MySQL Server
- IntelliJ IDEA, Eclipse, or another Java IDE
- MySQL Connector/J JDBC driver

### Installation

**1. Clone the repository**

```bash
git clone https://github.com/YOUR-USERNAME/Core-Banking-System.git
```

**2. Navigate to the project directory**

```bash
cd Core-Banking-System
```

**3. Create the database**

Open MySQL Workbench or your MySQL command-line client and execute your database schema:

```sql
CREATE DATABASE bank_management;
USE bank_management;
```

Create the required tables using the SQL schema provided in the project.

**4. Configure the database connection**

Update your JDBC connection settings with your local MySQL credentials.

```java
String url = "jdbc:mysql://localhost:3306/bank_management";
String username = "your_username";
String password = "your_password";

Connection connection = DriverManager.getConnection(
    url, username, password
);
```

**Important:** Keep database credentials out of public repositories. Use environment variables or a configuration file excluded through `.gitignore` for sensitive values.

**5. Add the MySQL JDBC driver**

Add MySQL Connector/J to your project's dependencies or classpath.

**6. Run the application**

Open the project in your Java IDE, configure the dependencies, and run the main application class.

## 🖥️ Application Modules

The application is organized into multiple GUI modules covering common banking operations.

| Module | Description |
|---|---|
| Login | Entry point for authorized users, if implemented |
| Dashboard | Navigation to banking operations |
| Account Management | Customer and account-related operations |
| Deposit | Adds funds to an account |
| Withdrawal | Deducts funds from an account |
| Balance Enquiry | Displays the current account balance |
| Transaction History | Displays recorded transactions, if implemented |

## 🗄️ Database

MySQL is used to store and manage application data. JDBC connects the Java application to the database and enables SQL operations.

The database can include tables for:

- Customers
- Bank accounts
- Transactions
- User credentials, if authentication is implemented

Appropriate primary keys, foreign keys, and constraints can be used to maintain data integrity.

## 🎯 Key Learnings

- Applied object-oriented programming principles in Java.
- Developed desktop interfaces using Java Swing.
- Connected a Java application to MySQL using JDBC.
- Implemented CRUD operations and SQL queries.
- Worked with relational database design and data integrity.
- Improved query performance through SQL optimization.

## 🚀 Future Enhancements

- Add role-based access control for administrators and customers.
- Implement secure authentication and password hashing.
- Introduce transaction rollback and stronger transaction consistency.
- Add account statements and transaction filtering.
- Improve input validation and exception handling.
- Develop a web-based version with a modern frontend.

## 👩‍💻 Author

**Anadi Chouhan**

B.Tech Computer Science Engineering — Artificial Intelligence & Machine Learning

## 📄 License

This project is intended for educational and demonstration purposes. Add an appropriate open-source license if you plan to distribute it publicly.

---

⭐ If you find this project interesting, consider giving the repository a star!
