# Database Indexing and Optimization

## 📌 Overview

This assignment focuses on database indexing, user account management, access control, and database security using MySQL. It demonstrates how to remove an index, create a database user, grant specific privileges, and update a user's password.

## 🎯 Learning Objectives

- Understand how to manage database indexes.
- Create MySQL user accounts with specific host restrictions.
- Grant database privileges using SQL commands.
- Change user passwords securely.
- Understand basic database security and access control.

## 🛠️ Tools and Technologies

- **Database Management System:** MySQL
- **Database Tool:** MySQL Workbench
- **Language:** SQL

## 📝 Assignment Questions and Solutions

### Question 1: Drop an Index

**Task:** Write an SQL query to drop an index named `IdxPhone` from the `customers` table.

```sql
DROP INDEX IdxPhone ON customers;
```

**Explanation:** This command removes the `IdxPhone` index from the `customers` table.

### Question 2: Create a Database User

**Task:** Create a user named `bob`, restricted to localhost, with the assigned password.

```sql
CREATE USER 'bob'@'localhost'
IDENTIFIED BY '_S$cu3r3!';
```

**Explanation:** This command creates the MySQL user `bob`, who can connect from the local database server.

### Question 3: Grant INSERT Privileges

**Task:** Grant the `INSERT` privilege to `bob` on the `salesDB` database.

```sql
GRANT INSERT ON salesDB.* TO 'bob'@'localhost';
```

**Explanation:** This command allows `bob` to insert records into tables within the `salesDB` database.

### Question 4: Change the User Password

**Task:** Change the password for the user `bob`.

```sql
ALTER USER 'bob'@'localhost'
IDENTIFIED BY 'P$55!23';
```

**Explanation:** This command changes the password for the existing MySQL user `bob`.

## ▶️ How to Execute the Queries

1. Open MySQL Workbench.
2. Connect to your MySQL server using an account with sufficient privileges.
3. Open a new SQL query tab.
4. Copy the queries into your `answers.sql` file.
5. Execute the queries in the correct order.
6. Check the output for successful execution and any errors.

## 📂 Project Structure

```text
database-indexing-optimization/
├── README.md
└── answers.sql
```

- `README.md` contains the assignment overview, objectives, and explanations.
- `answers.sql` contains the SQL solutions for all four questions.

## 🔐 Security Considerations

- Restrict database users to the hosts they need.
- Grant only the privileges required for their work.
- Use strong, unique passwords.
- Avoid sharing database credentials publicly or committing real passwords to public repositories.

## ✅ Conclusion

This assignment provides practical experience in MySQL index management, user creation, privilege assignment, and password modification. These skills help improve database administration, security, and access control.

---

**Author:** Silvio Ukoth Ukoro  
**Course/Module:** Database Indexing and Optimization  
**Database System:** MySQL
