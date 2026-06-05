# Sistem Informasi Perpustakaan

Web-based library management system built with PHP and CodeIgniter.

## Overview

This application supports library operations such as member management, book inventory, borrowing, returns, and staff notifications. It includes role-based access control for `admin` and `petugas` users.

## Features

- User login with role support
  - `admin`: full access to data management and system settings
  - `petugas`: access to borrowing and returning workflows only
- Member management (CRUD)
- Book management (CRUD)
- Borrowing and return transactions
- Notification system for admin to notify staff
- Dashboard and reporting components

## Technology stack

- PHP
- CodeIgniter
- MySQL / MariaDB
- HTML/CSS/JavaScript
- Bootstrap

## Requirements

- PHP 5.2.4 or higher
- MySQL / MariaDB
- Web server (Apache, Nginx, etc.)

## Installation

1. Copy the project into your web server document root.
2. Import the database using `assets/perpustakaan.sql`.
3. Update `application/config/database.php` with your database credentials.
4. Set `base_url` in `application/config/config.php` to match your environment.
5. Ensure `application/cache` and `application/logs` are writable by the web server.

## Database

- Database file: `assets/perpustakaan.sql`
- Default database name: `perpustakaan`

## Notes before publishing to GitHub

- Add a root `.gitignore` file to exclude runtime cache and logs.
- Do not commit sensitive database credentials.
- Consider renaming `license.txt` to `LICENSE` if you want GitHub to detect the license automatically.

## License

This project uses the MIT License.
