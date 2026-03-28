# 🥋 DojoMaster v1.0: Martial Arts Management System

**DojoMaster** is a simple and efficient software built to manage a Martial Arts Dojo. It helps in keeping records of members, their attendance, and fee status using **Python** and **MySQL**.

---

## 🚀 Main Features

* **Member Management**: Easily Add, View, or Delete members from the system.
* **Attendance Tracker**: Records daily attendance automatically using the current date.
* **Fee Tracking**: Keeps a simple record of whether a member has "Paid" or has "Pending" fees.
* **Smart Reports**: Generates a "Monthly Attendance " report to see top-performing students.
* **File Export**: Saves all reports into a `.txt` file so you can print or view them offline.

---

## 🛠️ How it Works (Technical Details)

### 1. Fast Performance (Database + List)
Instead of asking the Database for information again and again, the system loads all members into a **Python List** when it starts. This makes the software run very fast while keeping the data safe in the **MySQL Database**.

### 2. Security (SQL Injection Protection)
The system uses `%s` placeholders for all database commands. This is a security feature that prevents hackers from entering wrong commands into your database.

### 3. Smart SQL Queries
It uses **SQL JOINs** to connect the 'Member table' with the 'Attendance table'. This helps in creating detailed reports about each student's progress.

---

## 💻 Skills & Concepts Used

| Concept | What it does? |
| :--- | :--- |
| **Python OOPs** | Used Classes and Objects to keep the code organized. |
| **MySQL** | Used as a permanent storage for all member data. |
| **Error Handling** | Used `try-except` so the program doesn't crash if someone types wrong data. |
| **File Handling** | Used `with open()` to save reports directly to a text file. |

---

## 📂 How to Setup
1. Create a MySQL database named `DOJOMASTER`.
2. Install the MySQL connector: `pip install mysql-connector-python`.
3. Run the project: `python Dojo_Master.py`.

---
**Developed by:** Rajat Bhatt  
*B.Tech CSE Student | Martial Arts Practitioner*
