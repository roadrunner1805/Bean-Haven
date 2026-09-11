# Dynamic Web Application & Authentication System 🌐

A collaborative web development project built to practice core full-stack web architecture, reusable templating, and session-based user authentication using PHP, HTML5, and CSS3.

Developed as a hands-on coursework project to demonstrate modular code organization, state management, and protected routing.

---

## 🛠️ Built With

* **Backend:** PHP
* **Frontend:** HTML5, CSS3 (`style.css`)
* **Architecture:** Modular server-side rendering (Header/Footer layout pattern)
* **Environment:** Apache Web Server (XAMPP / MAMP / LAMP or built-in PHP CLI)

---

## ✨ Key Features & Architecture

* **Modular UI Components (`header.php`, `footer.php`):** Reusable layout partials included across views using server-side PHP to keep markup DRY (*Don't Repeat Yourself*).
* **Protected Routing & Session Handling (`privatehome.php`):** Implements restricted-access views that verify active user sessions before rendering protected dashboard content.
* **Authentication Flow (`login.php`, `handler.php`, `logout.php`):** 
  * `login.php`: Captures user credentials through form inputs.
  * `handler.php`: Processes incoming `POST` requests, validates user session state, and directs authenticated users to the internal dashboard.
  * `logout.php`: Clears session data and safely redirects back to the public view.
* **Custom Styling (`style.css`):** Responsive stylesheet providing clean layout scaffolding and UI component styling.

---

## 📂 File Overview

```plaintext
├── index.php          # Main public landing view
├── login.php          # User login interface
├── handler.php        # Form processing and authentication logic
├── privatehome.php    # Restricted dashboard view for authenticated users
├── logout.php         # Session termination and cleanup script
├── header.php         # Reusable site header and navigation partial
├── footer.php         # Reusable site footer partial
├── style.css          # Core stylesheet
└── README.md          # Project documentation
