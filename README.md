# Laravel Library Management System

A Laravel web application for managing a library catalogue, members, and book loans. The interface includes role-aware access for administrators, staff, and members.

## Features

- Book and category management, search, and availability tracking
- Member records, member cards, and loan history
- Loan creation, quick loan and return flows, and overdue tracking
- Dashboard statistics and reports for circulation and transactions
- Role-based access for admin, staff, and member accounts

## Stack

- PHP 8.2+
- Laravel 12
- Node.js and npm with Vite and Tailwind CSS
- SQLite or another database supported by Laravel

## Local setup

    git clone https://github.com/Rimaestro/laravel-library-management-system.git
    cd laravel-library-management-system
    composer install
    npm install

Copy .env.example to .env and configure your database, then prepare and start the application:

    cp .env.example .env

    php artisan key:generate
    php artisan migrate --seed
    npm run build
    php artisan serve

Visit http://127.0.0.1:8000. The database seeder creates development accounts with a shared default password. Change those credentials before using a non-local environment.

## Tests

    php artisan test

## Project structure

- app/Http/Controllers/ — authentication, books, members, loans, dashboards, reports, and search
- app/Models/ — books, categories, members, and loans
- database/migrations/ and database/seeders/ — schema and sample data
- resources/views/ — Blade pages
- routes/web.php — application routes
- tests/ — Laravel test suite

## License

No license file is currently included. Reuse and redistribution are not granted unless the project owner adds a license.

