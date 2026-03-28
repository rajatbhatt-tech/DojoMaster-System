# 🥋 DojoMaster v1.0: Martial Arts Management System

**DojoMaster** is a specialized management application designed to streamline the administrative operations of a Martial Arts Dojo. Developed using **Python** and **MySQL**, the system focuses on data integrity, operational efficiency, and secure record-keeping.

---

## 🚀 Key Modules & Functionalities

* **Member Administration**: Facilitates comprehensive CRUD (Create, Read, Update, Delete) operations for member profiles, including age and belt level tracking.
* **Automated Attendance Logging**: Features a digital ledger system that captures real-time attendance using system timestamps.
* **Financial Management**: Provides a streamlined interface for tracking and updating membership fee statuses.
* **Relational Reporting**: Utilizes advanced SQL queries to generate monthly performance and attendance leaderboards.
* **Data Persistence & Export**: Includes functionality to generate formatted `.txt` reports for offline auditing and permanent storage.

---

## 🛠️ Technical Architecture & Optimization

### 1. Hybrid Data Management (Persistence vs. Performance)
The system architecture implements a dual-layer data handling strategy:
* **Database Persistence**: Uses MySQL for permanent, reliable data storage.
* **Local Caching**: Loads data into Python lists during object instantiation (`__init__`) to minimize redundant database queries and ensure a high-performance user experience.

### 2. Security Protocol (SQL Injection Mitigation)
To safeguard the system against malicious attacks, all database interactions are conducted via **Parameterized Queries**. By using `%s` placeholders, the system ensures that user input is never executed as a database command.

### 3. Relational Intelligence
The reporting engine leverages **LEFT JOIN** operations and **SQL Aggregation** (`COUNT` & `GROUP BY`) to correlate data across multiple tables, providing accurate insights into member activity.

---

## 💻 Tech Stack & Engineering Concepts

| Concept | Technical Implementation | Purpose |
| :--- | :--- | :--- |
| **Encapsulation** | Class `Dojo` | Binding data and functions into a modular unit. |
| **State Initialization** | `__init__` | Automated session and data setup upon object creation. |
| **Error Resilience** | `try-except` Blocks | Robust exception handling to manage runtime data-type mismatches. |
| **Resource Management** | `with open()` | Efficient file stream handling for automated resource cleanup. |

---

## 📂 Installation & Setup
1. Initialize a MySQL database named `DOJOMASTER`.
2. Configure the database connector credentials in the source code.
3. Install dependencies: `pip install mysql-connector-python`.
4. Execute the application: `python Dojo_Master.py`.

---
**Developed by:** Rajat Bhatt  
*Software Engineering Candidate | Specialized in Python & Relational Databases*
