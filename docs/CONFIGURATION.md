# Configuration Guide

## Database Setup

### SQLite (Default)
No configuration needed. Database file created automatically.

### PostgreSQL

1. Install PostgreSQL 12+
2. Create database and user
3. Update `.env`:
```
DB_CONNECTION=pgsql
DB_HOST=127.0.0.1
DB_PORT=5432
DB_DATABASE=notes_api
DB_USERNAME=postgres
DB_PASSWORD=yourpassword
```

4. Run migrations:
```bash
php artisan migrate
```
