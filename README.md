# API-Call

## Project description

API-Call is a RESTful API built with Laravel for managing student data. This project provides complete CRUD (Create, Read, Update, Delete) operations for student records, allowing you to insert, fetch, modify, and delete student information. The API can be tested using Postman for all HTTP methods.

### Features

- **Create (POST)**: Add new student records with name, email, and course information
- **Read (GET)**: Retrieve all students or fetch a specific student by ID
- **Update (PUT)**: Modify existing student records
- **Delete (DELETE)**: Remove student records from the database
- **Validation**: Built-in validation for required fields and unique email addresses
- **Error Handling**: Proper HTTP status codes and error messages

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
   git clone [YOUR_GITHUB_REPOSITORY_LINK]
   cd api-call
   ```

2. **Install Composer Dependencies**
   ```bash
   composer install
   ```

3. **Create Environment File**
   ```bash
   cp .env.example .env
   ```

4. **Generate Application Key**
   ```bash
   php artisan key:generate
   ```

5. **Set Up Database**
   ```bash
   php artisan migrate
   ```

6. **Start the Development Server**
   ```bash
   php artisan serve
   ```

   The API will be available at `http://localhost:8000`

### Verifying the Setup

Once the server is running, you can test the API by:
- Opening Postman
- Testing the endpoints listed below
- Creating, retrieving, updating, and deleting student records

### API Endpoints

- `GET /api/students` - Get all students
- `GET /api/students/{id}` - Get a specific student
- `POST /api/students` - Create a new student
- `PUT /api/students/{id}` - Update a student
- `DELETE /api/students/{id}` - Delete a student

### Testing with Postman

Import the API endpoints into Postman and test all CRUD operations. Student creation requires:
- `name` (string, required)
- `email` (email, required, unique)
- `course` (string, required)

## Screen Recording Demonstration

[Add your Google Drive link here]

