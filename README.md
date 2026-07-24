# MediCare Plus — Hospital Management System

> **Your Health, Our Priority**

A full-featured Hospital Management System built with **PHP**, **MySQL**, and **Bootstrap**. MediCare Plus streamlines the workflow between patients, doctors, and administrators — from appointment booking to prescription management and PDF report generation.

---

## Features

- Patient self-registration and appointment booking
- Doctor dashboard to view and manage appointments
- Admin panel to oversee patients, doctors, appointments, and feedback
- In-app chatbot for basic patient guidance
- PDF prescription generation using TCPDF
- Search functionality for patients, doctors, and messages
- Appointment cancellation by both patients and doctors
- Doctor management (add/remove) by admin
- Contact/feedback form with admin view
- Multi-theme and color scheme support

---

## Tech Stack

| Layer | Technology |
|---|---|
| Frontend | HTML5, CSS3, Bootstrap 4, JavaScript |
| Backend | PHP 7+ |
| Database | MySQL |
| PDF Generation | TCPDF |
| Rich Text | CKEditor |
| Local Server | XAMPP (Apache + MySQL) |

---

## Prerequisites

Before running this project, make sure you have the following installed:

1. **XAMPP** (includes Apache and MySQL) — [Download here](https://www.apachefriends.org/)
2. A code editor such as **VS Code** or **Sublime Text**
3. Any modern web browser (Chrome, Firefox, Edge)

---

## Getting Started

Follow these steps to set up the project on your local machine:

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR_USERNAME/Medicare-plus.git
```

### 2. Move Files to XAMPP

Copy the project folder into the `htdocs` directory of your XAMPP installation:

- **Windows:** `C:\xampp\htdocs\`
- **Linux/macOS:** `/opt/lampp/htdocs/`

### 3. Start XAMPP Services

Open the XAMPP Control Panel and start both **Apache** and **MySQL**.

### 4. Set Up the Database

1. Open your browser and go to `http://localhost/phpmyadmin`
2. Create a new database named: `myhmsdb`
3. Select the database, go to the **Import** tab
4. Import the file: `myhmsdb.sql` (found in the project root)
5. Click **Go**

### 5. Launch the Application

Open your browser and navigate to:

```
http://localhost/Medicare-plus/
```

---

## Default Admin Credentials

```
Username: admin
Password: admin123
```

> ⚠️ **Change these credentials immediately** in a production environment.

---

## Project Structure

```
Medicare-plus/
├── index.php               # Home page (Patient/Doctor/Admin login & Patient Registration)
├── admin-panel.php         # Admin dashboard
├── doctor-panel.php        # Doctor dashboard
├── func.php                # Core logic & database handlers
├── func1.php / func2.php   # Additional function files
├── chatbot.php             # Chatbot interface
├── prescribe.php           # Prescription management
├── myhmsdb.sql             # Database schema and seed data
├── assets/                 # JS, CSS, images
├── TCPDF/                  # PDF generation library
├── vendor/                 # CKEditor and other vendors
└── README.md
```

---

## Modules

### Patient Module
- Register a new account
- Log in and access personal dashboard
- Book appointments with available doctors
- View appointment history and status
- Cancel upcoming appointments

### Doctor Module
- Log in to personal dashboard
- View all assigned patient appointments
- Search patients by contact number
- Cancel appointments

### Admin Module
- View and manage all registered patients
- View and manage all registered doctors (add / remove)
- View all appointment records
- Read user feedback and queries submitted via the Contact page

---

## Planned Improvements

- [ ] Doctor appointment approval/rejection with patient notification
- [ ] Prevent duplicate registration with the same email address
- [ ] Implement password hashing (bcrypt)
- [ ] Add pagination across all list views
- [ ] Fix billing receipt duplication for repeated doctor visits
- [ ] Expand prescription form with more clinical fields
- [ ] Add payment details (date, amount, method) to billing section
- [ ] Admin export to Excel for patient/doctor/appointment data

---

## Known Issues

- Passwords are currently stored in plain text — **do not use real credentials** in development.
- Bill payment receipt may show duplicate records if a patient visits the same doctor more than once.

---

## License

This project is open-source and available under the [MIT License](LICENSE).

---

## Author

Developed by **Prakhar Agrawal**
