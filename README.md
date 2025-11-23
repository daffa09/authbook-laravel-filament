<!-- portfolio -->
<!-- slug: authbook-laravel-filament -->
<!-- title: AuthoBook Management System -->
<!-- description: Book authentication and management system built with Laravel 10 and Filament admin panel -->
<!-- image: https://github.com/user-attachments/assets/de85ddfe-de3c-46dc-9cfa-0d77efd628f3 -->
<!-- tags: laravel, filament, php, authentication, admin-panel -->

# AuthBook Laravel 10 with Filament

<img width="1536" height="1024" alt="authbook-laravel-filament" src="https://github.com/user-attachments/assets/de85ddfe-de3c-46dc-9cfa-0d77efd628f3" />

A comprehensive book authentication and management system built with Laravel 10 and Filament admin panel. This project serves as a learning example for implementing modern admin panels with Filament in Laravel applications, created for the Web Programming (PBW) class.

## 📋 Overview

AuthBook is a full-featured book management system that demonstrates the integration of Laravel 10 with Filament admin panel. The project showcases best practices in building CRUD (Create, Read, Update, Delete) applications with authentication, authorization, and a modern admin interface.

## ✨ Features

- **User Authentication & Authorization**
  - Secure login/logout system
  - Role-based access control
  - User profile management

- **Book Management**
  - Complete CRUD operations for books
  - Book categorization and tagging
  - Advanced search and filtering
  - Bulk actions support

- **Modern Admin Panel (Filament)**
  - Beautiful, responsive UI
  - Customizable dashboard
  - Resource management
  - Form builders and tables
  - Notifications and widgets

- **Database Management**
  - MySQL database integration
  - Eloquent ORM relationships
  - Database migrations and seeders

## 🛠️ Technologies Used

- **Framework**: Laravel 10
- **Admin Panel**: Filament v3
- **Language**: PHP 8.1+
- **Database**: MySQL
- **Frontend**: Livewire, Alpine.js, Tailwind CSS
- **Authentication**: Laravel Breeze/Sanctum

## 📁 Project Structure

```
authbook-laravel-filament/
├── app/
│   ├── Filament/              # Filament resources
│   ├── Models/                # Eloquent models
│   └── Policies/              # Authorization policies
├── database/
│   ├── migrations/            # Database migrations
│   └── seeders/               # Database seeders
├── resources/
│   └── views/                 # Blade templates
├── routes/
│   └── web.php               # Web routes
└── config/
    └── filament.php          # Filament configuration
```

## 🚀 Getting Started

### Prerequisites

- PHP 8.1 or higher
- Composer
- MySQL 5.7+ or MariaDB
- Node.js & NPM (for asset compilation)

### Installation Steps

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd authbook-laravel-filament
   ```

2. **Install PHP dependencies**
   ```bash
   composer install
   ```

3. **Install Node dependencies**
   ```bash
   npm install
   ```

4. **Environment Setup**
   ```bash
   cp .env.example .env
   php artisan key:generate
   ```

5. **Configure Database**
   - Create a MySQL database
   - Update `.env` file:
   ```env
   DB_CONNECTION=mysql
   DB_HOST=127.0.0.1
   DB_PORT=3306
   DB_DATABASE=authbook_db
   DB_USERNAME=root
   DB_PASSWORD=your_password
   ```

6. **Run Migrations & Seeders**
   ```bash
   php artisan migrate --seed
   ```

7. **Create Admin User**
   ```bash
   php artisan make:filament-user
   ```
   Follow the prompts to create your admin account

8. **Build Assets**
   ```bash
   npm run dev
   ```

9. **Start Development Server**
   ```bash
   php artisan serve
   ```

10. **Access the Application**
    - Frontend: `http://localhost:8000`
    - Admin Panel: `http://localhost:8000/admin`

## 💻 Usage

### Accessing Admin Panel

1. Navigate to `http://localhost:8000/admin`
2. Login with your admin credentials created earlier
3. Access the dashboard to manage books and users

### Managing Books

1. Click on "Books" in the admin sidebar
2. Use "New Book" button to add books
3. Fill in book details (title, author, ISBN, description, etc.)
4. Click "Create" to save

### User Management

1. Access "Users" from the admin panel
2. View, edit, or delete users
3. Assign roles and permissions

## 🎓 Learning Objectives

This project demonstrates:

- **Filament Integration**: How to integrate and customize Filament admin panel
- **Resource Management**: Creating Filament resources for CRUD operations
- **Authentication**: Implementing secure user authentication
- **Authorization**: Role-based access control
- **Database Relationships**: Eloquent relationships and migrations
- **Modern PHP**: Latest PHP 8.1+ features and Laravel best practices

## 📚 Filament Resources

The project includes example Filament resources for:
- Book management
- User administration
- Category management
- Dashboard widgets

## 🔧 Configuration

### Filament Customization

Edit `config/filament.php` to customize:
- Brand name and logo
- Color scheme
- Navigation items
- Middleware and guards

### Database Seeders

The project includes seeders for:
- Sample books
- Demo users
- Categories and tags

Run seeders with:
```bash
php artisan db:seed
```

## 🤝 Contributing

This project is used for educational purposes in the Web Programming class. Contributions to improve the examples and documentation are welcome!

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Open a Pull Request

## 📄 License

This project is open source and available for educational purposes.

## 📖 Resources

- [Laravel Documentation](https://laravel.com/docs)
- [Filament Documentation](https://filamentphp.com/docs)
- [Livewire Documentation](https://livewire.laravel.com/docs)

## 📞 Contact

For questions about this learning project, please contact through the information available in my portfolio.
