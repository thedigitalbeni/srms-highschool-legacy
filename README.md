# 🎓 Student Result Management System (SRMS)

![PHP](https://img.shields.io/badge/PHP-7.4+-777BB4?style=for-the-badge&logo=php&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-8.0+-4479A1?style=for-the-badge&logo=mysql&logoColor=white)
![Gulp](https://img.shields.io/badge/Gulp-Task_Runner-EB4A4B?style=for-the-badge&logo=gulp&logoColor=white)
![Sass](https://img.shields.io/badge/Sass-Styles-CC6699?style=for-the-badge&logo=sass&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green.svg?style=for-the-badge)

> A powerful, automated, and secure web application designed to digitize school academic records and streamline result management.

---

## 🌟 Introduction

The **Student Result Management System (SRMS)** is a high-school portfolio project developed to solve the inefficiencies of manual grading and result distribution. This system provides a robust platform for school administrators to manage students, subjects, and classes while offering a seamless experience for students to access their performance reports instantly.

It features a modern, responsive administrative dashboard and a student-facing portal with PDF generation capabilities.

---

## 🚀 Key Features

### 👨‍💼 Administrator Module
The "Brain" of the system. Admins have total control over the academic data.
*   **🔐 Secure Authentication:** Multi-layered login system to protect sensitive student data.
*   **👥 Student Management:** 
    *   Register new students with unique Roll IDs.
    *   Edit student details or manage their active/inactive status.
*   **📚 Subject Management:**
    *   Create subjects with unique codes.
    *   Manage "Subject Combinations" (linking subjects to specific classes).
*   **🏫 Class Management:** Create and edit classes and sections (e.g., Class 10 - Section A).
*   **📊 Result Engine:**
    *   Input marks for individual students based on their class/subject.
    *   Update or correct marks at any time.
    *   Automated calculation of results.

### 🎓 Student Module
A simplified, user-friendly interface for students.
*   **🔍 Instant Search:** Find results using only Roll ID and Class selection.
*   **📄 PDF Generation:** Integrated with `dompdf` to allow students to download professional, formatted result sheets.
*   **📱 Fully Responsive:** Optimized for mobile, tablet, and desktop viewing.

---

## 🛠 Technical Architecture

### **The Backend Engine**
*   **PHP (PDO):** Uses PHP Data Objects for database interactions, ensuring protection against **SQL Injection**.
*   **MySQL:** A relational database structure with optimized tables for `students`, `classes`, `subjects`, and `results`.

### **The Asset Pipeline**
This isn't just a basic PHP site. It includes a modern development workflow:
*   **Sass (SCSS):** Advanced styling with variables and nesting.
*   **Gulp:** Automated tasks for:
    *   Compiling SCSS to CSS.
    *   Autoprefixing CSS for browser compatibility.
    *   Minifying JavaScript and CSS for faster load times.
    *   Browser-sync for real-time development.

### **Frontend & UI**
*   **Bootstrap 3:** For a solid, responsive grid system.
*   **Animate.css:** For smooth UI transitions and entry effects.
*   **Lobipanel & Toastr:** For elegant dashboard widgets and non-intrusive notifications.

---

## 📂 Project Structure

```text
├── css/              # Compiled & Minified CSS
├── js/               # Frontend Logic & Vendor Scripts
├── sass/             # Source SCSS files
├── db/               # Database Schemas (srms.sql)
├── includes/         # Core configuration & Reusable UI components
├── dompdf/           # PDF Generation Library
├── images/           # System assets and backgrounds
├── gulpfile.babel.js # Gulp automation configuration
└── package.json      # Node.js dependencies
```

---

## ⚙️ Installation & Local Setup

Ready to get this running? Follow these steps:

### 1️⃣ Prerequisites
*   **Server:** XAMPP, WAMP, or Laragon.
*   **PHP:** v7.0 or higher.
*   **Database:** MySQL.
*   **Node.js:** (Optional) If you want to use the Gulp build system.

### 2️⃣ Database Setup
1.  Open **phpMyAdmin**.
2.  Create a new database named `srms`.
3.  Import the file `/db/srms.sql` into the newly created database.

### 3️⃣ Configuration
Update the database connection details in both:
*   `includes/config.php`
*   `includes/configpdo.php`

```php
define('DB_HOST','localhost');
define('DB_USER','root');
define('DB_PASS','');
define('DB_NAME','srms');
```

### 4️⃣ Launch
Move the folder to your server's root (e.g., `htdocs`) and visit:
`http://localhost/student-result-management-system/`

---

## 🎨 UI Preview

| Admin Dashboard |
| :--- | :--- |
| ![Dashboard](<img width="1366" height="553" alt="Screenshot from 2026-06-16 09-38-40" src="https://github.com/user-attachments/assets/9b47047f-b4b0-437e-9643-e0ea5b0cd28b" />
) | 

*(Note: Replace placeholders with actual screenshots for a better GitHub profile!)*

---

## 🛡️ License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

---

## ✍️ Author

**Beneyas**
*   🚀 **High School Legacy Project:** I built this system when I was in **Grade 11** for my own school! It was one of my first major projects, designed to solve real-world problems in my student community.
*   📫 Connect with me if you have questions or want to talk about early-career dev stories!

---
*If you like this project, don't forget to give it a ⭐!*
