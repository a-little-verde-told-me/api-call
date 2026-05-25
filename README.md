# API-Call

## Project description

API-Call is a RESTful API built with Laravel for managing student data. This project provides complete CRUD (Create, Read, Update, Delete) operations for student records, allowing you to insert, fetch, modify, and delete student information. The API can be tested using Postman for all HTTP methods.

### Features

- **Create (POST)**: Add new student records with name, email, and course information
- **Read (GET)**: Retrieve all students or fetch a specific student by ID
- **Update (PUT and PATCH)**: Modify existing student records
- **Delete (DELETE)**: Remove student records from the database

## Setup Instructions

### Prerequisites

- PHP 8.2 or higher
- Composer
- Laravel 11.x
- SQLite or MySQL database
- Postman (for testing the API)

### Installation Steps

1. **Clone the Repository**
   ```bash
   git clone https://github.com/a-little-verde-told-me/api-call.git
   cd api-call
   ```

2. **Install Composer Dependencies**
   ```bash
   composer install
   ```

3. **Create .env File**
   ```bash
   cp .env.example .env
   ```

4. **Generate Application Key**
   ```bash
   php artisan key:generate
   ```

5. **Run a migration**
   ```bash
   php artisan migrate
   ```

6. **Start the Development Server**
   ```bash
   php artisan serve
   ```
7. **Test the API in Postman**
   ```bash
   http://127.0.0.1:8000/api/students
   ```


### Verifying the Setup

Once the server is running, you can test the API by:
- Opening Postman
- Testing the endpoints listed below
- Inserting, fetching, updating, and deleting student records

### API Endpoints

- `GET /api/students` - Get all students
- `GET /api/students/{id}` - Get a specific student
- `POST /api/students` - Insert a new student
- `PUT /api/students/{id}` - Modify a student (this requires to use all the required fields)
- `PATCH /api/students/{id}` - Update a student (just the field you want to update)
- `DELETE /api/students/{id}` - Delete a specific student
- `DELETE /api/students` - Delete all student

### Testing with Postman

Import the API endpoints into Postman and test all CRUD operations. Student creation requires:
- `name` (string, required)
- `email` (email, required, unique)
- `course` (string, required)

## Screen Recording Demonstration

https://drive.google.com/drive/folders/1cGIuKlq5YHQF1CJvfnGRWUnXw1AVkBZC?usp=sharing

