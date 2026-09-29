# Laravel Notes API

A small REST API for managing notes, built with Laravel 11 and Eloquent. Supports SQLite (default, zero-config) or PostgreSQL.

## Endpoints

| Method | Path              | Description       |
|--------|-------------------|--------------------|
| GET    | /api/notes        | List all notes     |
| POST   | /api/notes        | Create a note       |
| GET    | /api/notes/{id}   | Get a single note  |
| PUT    | /api/notes/{id}   | Update a note       |
| DELETE | /api/notes/{id}   | Delete a note       |

## Setup

```bash
composer install
cp .env.example .env
php artisan key:generate
touch database/database.sqlite
php artisan migrate
php artisan serve
```

To use PostgreSQL instead of SQLite, uncomment the `DB_*` lines in `.env` and comment out the SQLite ones.

## Stack

- Laravel 11
- Eloquent ORM
- SQLite / PostgreSQL
- RESTful resource routing (`Route::apiResource`)
