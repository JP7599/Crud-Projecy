# PHP CRUD Application

A simple and elegant CRUD (Create, Read, Update, Delete) application built with PHP and MySQL. This application features a modern, responsive design with a clean user interface for managing user data.

## Features

- Create new user records
- View all users in a responsive table
- Update existing user information
- Delete user records
- Form validation
- Responsive design using Bootstrap
- Success/Error notifications
- Clean and intuitive interface

## Technologies Used

- PHP 7+
- MySQL
- Bootstrap 4.0
- HTML5
- CSS3

## Prerequisites

Before you begin, ensure you have the following installed:
- XAMPP (or similar local server environment)
- Web browser
- Text editor (VS Code recommended)

## Installation

1. Clone the repository
```bash
git clone https://github.com/JP7599/Crud-Projecy.git
```

2. Move the project to your local server directory
```bash
# For XAMPP (Windows)
Move the project folder to C:/xampp/htdocs/
```

3. Start your local server (XAMPP)
- Start Apache and MySQL services from XAMPP Control Panel

4. Create the database
- Open phpMyAdmin (http://localhost/phpmyadmin)
- Create a new database named `my_db`
- Import the database structure using this SQL:
```sql
CREATE TABLE users (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(255) NOT NULL,
    email VARCHAR(255) NOT NULL
);
```

5. Configure the database connection
- Open `db_conn.php`
- Verify these settings match your environment:
```php
$sname = "localhost";
$uname = "root";
$password = "";
$db_name = "my_db";
```

## Usage

1. Access the application:
- Open your web browser
- Navigate to: `http://localhost/your-project-folder`

2. Features:
- Click "Create" to add a new user
- View all users in the table
- Use "Update" to modify user information
- Use "Delete" to remove a user

## Project Structure

```
├── css/
│   └── style.css                # Custom styles
├── php/
│   ├── create.php              # Handle user creation
│   ├── read.php                # Fetch user data
│   ├── update.php              # Handle user updates
│   └── delete.php              # Handle user deletion
├── db_conn.php                 # Database connection
├── index.php                   # Main entry point
├── read.php                    # View all users
└── update.php                  # Update user form
```

## Security Features

- Input validation and sanitization
- HTML escaping to prevent XSS
- SQL injection prevention
- Form validation

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is open source and available under the [MIT License](LICENSE).

## Contact

Your Name - [@JP7599](https://github.com/JP7599)

Project Link: [https://github.com/JP7599/Crud-Projecy](https://github.com/JP7599/Crud-Projecy)