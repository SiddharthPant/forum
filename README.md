# Forum Application

A modern forum application built with Laravel and Vue.js, demonstrating full-stack development skills and exploring the complexity behind seemingly simple web applications.

## Project Overview

A forum is deceptively complex. Sure, it's made up of threads and replies, but what else might exist as part of a forum? What about profiles, or thread subscriptions, or filtering, or real-time notifications? As it turns out, a forum is the perfect project to stretch your programming muscles.

This project explores the intricacies of building a comprehensive forum system, implementing features that showcase modern web development practices and Laravel's powerful ecosystem.

## Tech Stack

-   **Backend**: Laravel 11 with PHP 8.2+
-   **Frontend**: Vue.js 3 with Inertia.js for seamless SPA experience
-   **Styling**: Tailwind CSS for modern, responsive design
-   **Authentication**: Laravel Jetstream with Sanctum
-   **Testing**: Pest for elegant PHP testing
-   **Code Quality**: Laravel Pint for consistent formatting

## Features Implemented

-   **Thread Management**: Create, edit, and organize discussion threads
-   **Reply System**: Nested replies with rich text support
-   **User Profiles**: Customizable user profiles with activity tracking
-   **Authentication**: Secure user registration and login
-   **Responsive Design**: Mobile-first approach with Tailwind CSS
-   **Real-time Updates**: Live notifications and updates (planned)
-   **Thread Subscriptions**: Follow interesting discussions (planned)
-   **Advanced Filtering**: Search and filter threads by various criteria (planned)

## Quick Start

### Prerequisites

-   PHP 8.2 or higher
-   Composer
-   Node.js & npm
-   SQLite (default) or MySQL/PostgreSQL

### Installation

1. **Clone the repository**

    ```bash
    git clone <repository-url>
    cd forum
    ```

2. **Install PHP dependencies**

    ```bash
    composer install
    ```

3. **Install JavaScript dependencies**

    ```bash
    npm install
    ```

4. **Environment setup**

    ```bash
    cp .env.example .env
    php artisan key:generate
    ```

5. **Database setup**

    ```bash
    touch database/database.sqlite
    php artisan migrate --seed
    ```

6. **Start development servers**

    ```bash
    # Terminal 1: Laravel backend
    php artisan serve

    # Terminal 2: Vite frontend
    npm run dev
    ```

7. **Visit the application**
   Open [http://localhost:8000](http://localhost:8000) in your browser

## Development Commands

-   `php artisan serve` - Start Laravel development server
-   `npm run dev` - Start Vite development server with hot reload
-   `npm run build` - Build assets for production
-   `php artisan test` - Run PHP tests using Pest
-   `./vendor/bin/pint` - Format PHP code with Laravel Pint

## Project Structure

```
├── app/                    # Laravel application logic
│   ├── Http/Controllers/   # Request handlers
│   ├── Models/            # Eloquent models
│   └── Policies/          # Authorization policies
├── database/              # Migrations, seeders, factories
├── resources/
│   ├── js/               # Vue.js components and frontend logic
│   └── views/            # Blade templates
├── routes/               # Route definitions
└── tests/               # Test files
```

## Why This Project?

Forums represent a perfect balance of complexity and familiarity. While the concept is simple, the implementation reveals numerous challenges:

-   **Data Relationships**: Users, threads, replies, and their interconnections
-   **Real-time Features**: Live updates and notifications
-   **User Experience**: Intuitive navigation and interaction patterns
-   **Performance**: Efficient querying and caching strategies
-   **Security**: Protecting against common web vulnerabilities
