
# Library Management System

## Overview

The **Library Management System** is a web application developed using PHP and MySQL, designed to streamline the operations of a library. This system manages books, members, and lending processes efficiently. Built with a user-friendly interface, it allows librarians to easily manage records, while members can search for and reserve books.

## Key Features

- **Member Management**: Add, update, and remove members.
- **Book Management**: Add, categorize, and manage books with details such as title, author, ISBN, and publisher.
- **Borrowing and Returning**: Record and track book borrowings, return dates, and calculate late fines.
- **Search and Filter**: Search books by various filters like title, author, category, etc.
- **Reservations**: Allow members to reserve books that are currently unavailable.
- **Reports and Statistics**: View reports on borrowed books, overdue books, and member activity.

## Technologies Used

- **Backend**: PHP (Server-side scripting)
- **Database**: MySQL (Database management)
- **Local Server**: XAMPP (Apache server, MySQL database, PHP interpreter)
- **Text Editor**: Sublime Text (Code development)

## Setup Instructions

Follow these steps to set up the Library Management System on your local machine:

### Prerequisites
- XAMPP installed on your system
- Sublime Text or any text editor of your choice

### Steps

1. **Clone the Repository**
   ```bash
   git clone https://github.com/yourusername/library-management-system.git
   ```
2. **Start XAMPP**
   - Open the XAMPP Control Panel.
   - Start the Apache and MySQL services.

3. **Database Setup**
   - Open [phpMyAdmin](http://localhost/phpmyadmin/) in your browser.
   - Create a new database, e.g., `library_db`.
   - Import the `library_db.sql` file located in the `db/` folder of the project to set up the necessary tables.

4. **Configure Database Connection**
   - Open the project folder in Sublime Text.
   - Navigate to `config.php` and update the following fields with your MySQL credentials:
     ```php
     define('DB_SERVER', 'localhost');
     define('DB_USERNAME', 'root');
     define('DB_PASSWORD', '');
     define('DB_DATABASE', 'library_db');
     ```

5. **Run the Application**
   - Move the project folder to the `htdocs` directory of your XAMPP installation (usually found at `C:/xampp/htdocs/`).
   - Open your browser and go to `http://localhost/library-management-system/`.

## Usage

1. **Librarian Dashboard**: After logging in, librarians can manage books, members, and transactions such as borrowings and returns.
2. **Member Portal**: Members can view available books, search, and reserve books.

## File Structure

```
library-management-system/
│
├── db/
│   └── library_db.sql          # Database schema
├── config.php                  # Database configuration file
├── index.php                   # Application entry point (login page)
├── dashboard.php               # Librarian dashboard
├── add_book.php                # Form to add a new book
├── add_member.php              # Form to add a new member
├── borrow_book.php             # Handle book borrowing
├── return_book.php             # Handle book returning
└── assets/
    └── css/                    # CSS stylesheets
    └── js/                     # JavaScript files
    └── images/                 # Images and icons
```

## Screenshots

1. **Login Page**

   ![Login Page](screenshots/login_page.png)

2. **Librarian Dashboard**

   ![Dashboard](screenshots/dashboard.png)

## Contributing

Contributions are welcome! Please follow the steps below to contribute:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature`).
3. Commit your changes (`git commit -m 'Add your feature'`).
4. Push to the branch (`git push origin feature/your-feature`).
5. Create a Pull Request.


Feel free to adjust the descriptions, features, or any specific paths and commands based on how your system is structured!
