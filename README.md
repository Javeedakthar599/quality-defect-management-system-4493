# Project Repository

## 🗄️ Database (SQLite)

The application uses **SQLite** as the database for lightweight, fast, and easy setup during development and demo environments. Despite its simplicity, the database schema is designed to support a complete defect management lifecycle.

---

### 🧩 Core Data Models

The database is structured around the following key entities:

* 🐞 **Defect**

  * Title, description
  * Severity (Critical / Major / Minor)
  * Priority (P1, P2, etc.)
  * Status (Open, In Analysis, Actions In Progress, Closed)
  * Production details (line, shift, part number)
  * Due date and timestamps

* 🧠 **Root Cause Analysis**

  * Stores structured **5-Why analysis**
  * Includes:

    * Why1 → Why5
    * Root cause summary
    * Immediate containment actions

* ✅ **Corrective Action**

  * Linked to a defect
  * Fields include:

    * Action title
    * Owner
    * Due date
    * Status (Open / In Progress / Completed)

* 📜
