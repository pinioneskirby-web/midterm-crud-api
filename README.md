# IDTerm CRUD API

## 1. Project Description

The IDTerm CRUD API is a backend application developed using Node.js, Express.js, TypeScript, TypeORM, and MySQL. It allows users to create, read, update, and delete user records through REST API endpoints.

The project demonstrates how backend technologies work together to manage data and communicate with a MySQL database. It also uses proper error handling to ensure reliable API operations.

## 2. Setup Instructions

Follow these steps to set up the project:

1. Install Node.js and MySQL.
2. Clone or download the project repository.
3. Open the project folder in Visual Studio Code.
4. Open the terminal.
5. Install the required dependencies:

```bash
npm install
```

6. Create a `.env` file in the project folder and configure your database:

```env
DB_HOST=localhost
DB_PORT=3306
DB_USERNAME=root
DB_PASSWORD=your_password
DB_DATABASE=midterm_api
```

7. Create the MySQL database:

```sql
CREATE DATABASE midterm_api;
```

8. Make sure your MySQL server is running.

## 3. How to Run the Application

1. Open the project in Visual Studio Code.
2. Make sure MySQL is running.
3. Open the terminal.
4. Run the application using:

```bash
npm run dev
```

5. Wait for the server to start successfully.
6. Open Postman to test the API endpoints.

The application will run on the configured server port.

## 4. API Endpoints Documentation

The API provides the following CRUD operations for managing users.

| Method | Endpoint | Description |
|---|---|---|
| GET | `/api/users` | Retrieve all users |
| GET | `/api/users/:id` | Retrieve a user by ID |
| POST | `/api/users` | Create a new user |
| PUT | `/api/users/:id` | Update an existing user |
| DELETE | `/api/users/:id` | Delete a user |

### Example POST Request

```json
{
  "name": "Kirby",
  "email": "kirby@gmail.com"
}
```

### Example Response

```json
{
  "message": "User created successfully"
}
```

*Note: The endpoint paths and request fields above are examples. Make sure they match your actual routes and User entity.*

## 5. Reflection

**1. What did you learn from this project?**

I learned how to build a REST API using Node.js, Express.js, TypeScript, and MySQL. I also learned how to perform CRUD operations and connect an application to a database using TypeORM.

**2. What challenges did you encounter?**

One of the challenges I encountered was configuring the MySQL database and fixing errors in my TypeScript code. Sometimes the application did not run properly, but I learned how to identify and solve the errors.

**3. How did you overcome these challenges?**

I overcame these challenges by reviewing my code, checking error messages, and following the correct setup instructions. I also used documentation and practiced troubleshooting.

**4. What did you learn about API development?**

I learned that API development is important for communication between the frontend, backend, and database. I also understood how HTTP methods such as GET, POST, PUT, and DELETE are used to manage data.

**5. How can you improve this project in the future?**

I can improve this project by adding user authentication, better error handling, data validation, and additional security features.