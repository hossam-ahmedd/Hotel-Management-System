# Hotel Management System

A PHP/MySQL Hotel Management System for room booking, admin management, payments, invoices, staff management, room management, and dashboard statistics. The project was developed as a Software Engineering final project following the Software Development Life Cycle (SDLC).

## Project Overview

The Hotel Management System is a web-based application designed to reduce manual hotel reservation and administration work. It provides two main roles:

- **User / Guest**
- **Admin / Staff**

Users can create an account, log in, view hotel information, and submit room reservations. Admins can manage bookings, confirm reservations, generate payment records, print invoices, manage rooms, manage staff, and view dashboard statistics.

## Features

### User Features

- User registration
- User login
- View hotel homepage
- View available rooms and facilities
- Submit room reservation
- Logout

### Admin / Staff Features

- Admin/staff login
- View dashboard statistics
- View and manage room bookings
- Confirm reservations
- Edit booking information
- Delete bookings
- Generate payment records
- Print invoices
- Manage room records
- Manage staff records
- Export booking data

## Technologies Used

- **Frontend:** HTML, CSS, Bootstrap, JavaScript
- **Backend:** PHP
- **Database:** MySQL / MariaDB
- **Local Server:** XAMPP
- **Database Tool:** phpMyAdmin

## System Requirements

Before running the project, make sure you have:

- XAMPP installed
- Apache server enabled
- MySQL server enabled
- A modern web browser

## Installation and Setup

### 1. Download or Clone the Repository

```bash
git clone https://github.com/your-username/hotel-management-system.git
```

Or download the project as a ZIP file and extract it.

### 2. Move the Project to XAMPP

Copy the project folder to:

```text
C:\xampp\htdocs\Hotel-Management-System
```

### 3. Start XAMPP Services

Open XAMPP Control Panel and start:

```text
Apache
MySQL
```

### 4. Create the Database

Open phpMyAdmin:

```text
http://localhost/phpmyadmin
```

Create a new database named:

```text
bluebirdhotel
```

### 5. Import the Database File

Import the SQL file:

```text
bluebirdhotel.sql
```

into the `bluebirdhotel` database.

### 6. Check Database Configuration

Make sure the database connection file contains the correct XAMPP default settings:

```php
$server = "localhost";
$username = "root";
$password = "";
$database = "bluebirdhotel";
```

### 7. Run the Project

Open the project in your browser:

```text
http://localhost/Hotel-Management-System/index.php
```

## Default Login Accounts

### Admin / Staff Login

```text
Email: Admin@gmail.com
Password: 1234
```

### User Login

```text
Email: test@gmail.com
Password: 123
```

Or create a new user account from the sign-up page.

## Main Project Files

```text
Hotel-Management-System/
│
├── index.php                  # User and staff login / user signup
├── home.php                   # User homepage and booking page
├── config.php                 # Database connection
├── bluebirdhotel.sql          # Database file
│
├── admin/
│   ├── admin.php              # Admin main page
│   ├── dashboard.php          # Dashboard statistics
│   ├── roombook.php           # Booking management
│   ├── roomconfirm.php        # Booking confirmation
│   ├── payment.php            # Payment management
│   ├── invoiceprint.php       # Invoice printing
│   ├── room.php               # Room management
│   └── staff.php              # Staff management
│
├── css/                       # Stylesheets
├── javascript/                # JavaScript files
└── image/                     # Project images
```

## Database Tables

The system uses the following main database tables:

| Table Name | Purpose |
|---|---|
| `signup` | Stores user account information |
| `emp_login` | Stores admin/staff login information |
| `room` | Stores room type and bedding data |
| `roombook` | Stores reservation details |
| `payment` | Stores payment and invoice details |
| `staff` | Stores staff records |

## SDLC Phases Applied

This project follows the Software Development Life Cycle:

1. **Requirements Analysis:** Identify the problem, users, features, functional requirements, and non-functional requirements.
2. **Specification:** Define clear system behavior, inputs, outputs, constraints, and expected results.
3. **Design:** Prepare UML diagrams, system architecture, database design, and module structure.
4. **Implementation:** Develop the system using PHP, MySQL, HTML, CSS, Bootstrap, and JavaScript.
5. **Testing:** Test login, booking, admin management, payment, invoice, room, and staff modules.
6. **Maintenance:** Plan future improvements, bug fixes, security updates, and scalability enhancements.

## UML Diagrams

The project documentation includes the following UML diagrams:

- Use Case Diagram
- Sequence Diagram
- Activity Diagram
- Class Diagram
- State Machine Diagram
- Component Diagram
- Package Diagram
- Collaboration Diagram

## Testing Summary

Main test cases include:

- User registration with valid data
- User login with valid and invalid credentials
- Room reservation submission
- Admin/staff login
- Booking confirmation
- Payment generation
- Invoice printing
- Room addition and deletion
- Staff addition and deletion
- Dashboard statistics display

## Future Improvements

- Add online payment gateway integration
- Add email confirmation after booking
- Add room availability checking before reservation
- Add password hashing using `password_hash()` and `password_verify()`
- Improve role-based access control
- Add customer booking history
- Add reports by month and year
- Improve mobile responsiveness
- Deploy the system online

## Security Notes

This project is intended for academic use. For production deployment, it should be improved by:

- Hashing user and admin passwords
- Applying prepared statements to all SQL queries
- Adding server-side input validation
- Adding access control for every admin page
- Securing database credentials
- Using HTTPS on deployment

## Authors

Developed by:

```text
[Hossam Ahmed]
[Antony Medhat]
[Moahmed Ibrahim]
[Youssef Whaid]
[Rawan Sherif]
```

## Course Information

```text
Course: Software Engineering
Project: Final Project
System: Hotel Management System
University: Alexandria National University
Faculty: Faculty of Computers and Data Sciences (Cybersecurity Department)
```

## License

This project is developed for educational purposes.
