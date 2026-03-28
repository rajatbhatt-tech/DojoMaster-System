# 🥋 DojoMaster v1.0: Martial Arts Management System

**DojoMaster** is a robust management system developed to automate the daily operations of a Martial Arts Dojo. [cite_start]Built with **Python** and **MySQL**, it bridges the gap between traditional discipline and modern technology. [cite: 1, 4, 13, 129]

---

## 🚀 Project Overview
This project handles member registrations, attendance tracking, fee management, and performance reporting. [cite_start]It is designed with **Object-Oriented Programming (OOP)** principles to ensure scalability and clean code. [cite: 16, 141, 142]

### Key Features:
* [cite_start]**Member Management:** Add, delete, and view member profiles (Name, Age, Belt Level). [cite: 21, 26, 75]
* [cite_start]**Attendance Tracking:** Automated daily attendance logs using system dates. [cite: 37, 44]
* [cite_start]**Relational Reporting:** Generates "Monthly Attendance King" reports using SQL JOINs. [cite: 51, 52, 57, 154]
* [cite_start]**Fee Management:** Real-time updates for fee status. [cite: 82, 83]
* [cite_start]**Data Export:** Generates official `.txt` reports for offline record-keeping. [cite: 66, 67, 72]

---

## 🛠️ Technical Architecture

### 1. Database Connectivity (The Bridge)
* [cite_start]Uses `mysql.connector` to establish a secure session between Python and the MySQL server. [cite: 6, 8, 131, 132]
* [cite_start]**Authentication:** Configured with host, user, and password for secure access. [cite: 10, 11, 12, 134]

### 2. Efficiency & Performance (Local Cache)
* [cite_start]**The Strategy:** The system uses both a **Database** (for persistence) and a **Python List** (for performance). [cite: 18, 93, 176]
* [cite_start]**Reasoning:** To avoid redundant DB queries, data is loaded into a local list during initialization (`__init__`), ensuring the UI remains fast while keeping the DB as the permanent source of truth. [cite: 15, 17, 147, 148]

### 3. Security (SQL Injection Prevention)
* [cite_start]Implements **Parameterized Queries** using `%s` placeholders. [cite: 23, 149, 150, 151]
* [cite_start]This ensures that user input is treated as text, preventing malicious SQL commands from being executed. [cite: 152, 153]

---

## 💻 Tech Stack & Concepts Used

| Concept | Technical Term | Purpose |
| :--- | :--- | :--- |
| **Encapsulation** | Class `Dojo` | [cite_start]Binding data and functions into one unit. [cite: 16, 141, 143] |
| **Constructor** | `__init__` | [cite_start]Automatic state initialization on object creation. [cite: 17, 145, 147] |
| **Relational Logic** | `LEFT JOIN` | [cite_start]Merging 'Member' and 'Attendance' tables for reports. [cite: 53, 57, 154, 155] |
| **Aggregation** | `COUNT` & `GROUP BY`| [cite_start]Summarizing member data for performance tracking. [cite: 55, 59, 159, 160] |
| **Error Handling** | `try-except` | [cite_start]Handling `ValueError` during data entry to prevent crashes. [cite: 119, 124, 164, 166, 168] |
| **Persistence** | `with open()` | [cite_start]Efficiently managing file streams to save reports. [cite: 68, 169, 171, 173] |

---

## 📂 How to Run
1. [cite_start]Ensure you have **MySQL** installed and a database named `DOJOMASTER` created. [cite: 13]
2. [cite_start]Install the connector: `pip install mysql-connector-python`. [cite: 6]
3. [cite_start]Run the script: `python Dojo_Master.py`. [cite: 4]
4. [cite_start]Follow the command-line prompts to manage your Dojo! [cite: 94, 99]

---
**Developed by:** Rajat Bhatt  
*Bridging Martial Arts Discipline with Software Engineering.*
