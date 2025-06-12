# Day 21 – SQL Injection (Module 13)

## 🔍 Topics Covered:

- **What is SQL?** 
  Structured Query Language (SQL) is a standard language used to communicate with databases and perform tasks like data retrieval, insertion, modification, and deletion.

- **What is a Database?** 
  A structured collection of data stored electronically. Common types include relational databases like MySQL, PostgreSQL, SQL Server, and Oracle.

- **What is SQL Injection (SQLi)?** 
  A web security vulnerability that allows an attacker to interfere with the queries an application makes to its database. SQLi can be used to view or manipulate data they are not supposed to access.

---

### 🧾 Common SQL Verbs:
- `SELECT` – retrieve data
- `INSERT` – insert new data
- `DELETE` – remove data
- `UPDATE` – modify data
- `DROP` – delete database objects
- `UNION` – combine results of two queries

---

### 🔑 Other Important Terms:
- `WHERE`, `AND`, `OR`, `NOT` – used for filtering data
- `ORDER BY` – sort the result
- `FROM` – specify the data source (table)

---

### ⚠️ Special Characters in SQL Injection:
- `'` (Single quote)
- `--` (Comment)
- `#` (Alternate comment)
- `;` (Statement separator)
- `"` (Double quote)

---

### 🧨 Types of SQL Injection:
- **In-band SQLi** (Classic) 
  - Error-based 
  - Union-based 
- **Inferential SQLi** (Blind) 
  - Boolean-based 
  - Time-based 
- **Out-of-band SQLi** 
  - Uses external connections like DNS or HTTP to retrieve data

---

### 🛡️ Mitigation Techniques:
- Use of **Prepared Statements** and **Parameterized Queries**
- Employing **ORMs** (Object-Relational Mappers)
- Strict **input validation and sanitization**
- Applying **least privilege** on database users
- Enabling **WAF (Web Application Firewall)**

---

### 🔧 Tools Introduced:
- **sqlmap** 
  A powerful open-source tool used for automating the process of detecting and exploiting SQL injection vulnerabilities and taking over database servers.

---

## 📝 Summary:

On **Day 21**, the module on **SQL Injection** was introduced. The theory covered the foundation of SQL, types of SQLi attacks, and their prevention. The class also introduced **sqlmap**, a CLI-based tool for exploiting SQLi vulnerabilities. A solid understanding of database structures and SQL commands was emphasized to better comprehend injection logic and its potential impact.

---
