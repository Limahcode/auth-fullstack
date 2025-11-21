# Auth Fullstack Application

A full-stack authentication application built with Laravel 12 and React.

## Tech Stack

**Backend:**
- Laravel 12
- Laravel Sanctum (API Authentication)
- MySQL

**Frontend:**
- React 18
- React Router
- Axios
- Tailwind CSS

## Setup Instructions

### Backend Setup

1. Navigate to backend directory:
```bash
cd backend
```

2. Install dependencies:
```bash
composer install
```

3. Create `.env` file:
```bash
cp .env.example .env
```

4. Generate application key:
```bash
php artisan key:generate
```

5. Configure database in `.env`:
```
DB_DATABASE=auth_fullstack
DB_USERNAME=root
DB_PASSWORD=
```

6. Run migrations:
```bash
php artisan migrate
```

7. Start server:
```bash
php artisan serve
```
### For testing the Backend API
### Frontend Setup

1. Navigate to frontend directory:
```bash
cd frontend
```

2. Install dependencies:
```bash
npm install
```

3. Start development server:
```bash
npm run dev
```

## Features

- User Registration
- User Login
- User Logout
- Forgot Pasword
- Protected Routes
- Dashboard
- JWT Token Authentication

## API Endpoints

- `POST /api/register` - Register new user
- `POST /api/login` - Login user
- `POST /api/logout` - Logout user (requires auth)
- `POST /api/resetpassword'
- `GET /api/user` - Get authenticated user (requires auth)