# User CRUD API

## Project Overview

This project implements a **RESTful API for managing users** with full CRUD functionality (Create, Read, Update, Delete). The API is built using **Node.js, Express.js, and MongoDB with Mongoose**.

The purpose of this project is to demonstrate backend development skills including REST API design, database integration, input validation, and API testing.

## Tech Stack

* Node.js
* Express.js
* MongoDB
* Mongoose
* dotenv
* Bruno (for API testing)

## Features

* Create a new user
* Retrieve all users
* Retrieve a specific user by ID
* Update user information
* Delete a user
* Input validation for required fields
* Proper HTTP status codes and responses

## Project Structure

user-crud-api
│
├── models
│   └── User.js
│
├── controllers
│   └── userController.js
│
├── routes
│   └── userRoutes.js
│
├── .env
├── .gitignore
├── package.json
├── server.js
└── README.md

## Installation and Setup

### 1. Clone the Repository

git clone <repository-url>
cd user-crud-api

### 2. Install Dependencies

npm install

### 3. Configure Environment Variables

Create a `.env` file in the root directory and add:

PORT=5000
MONGO_URI=mongodb://localhost:27017/usercrud

If using MongoDB Atlas:
MONGO_URI=mongodb+srv://username:password@cluster.mongodb.net/usercrud

### 4. Start the Server

npm run dev

Server will run on:

http://localhost:5000

## API Endpoints

### Create User

**POST** `/api/users`


### Get All Users

**GET** `/api/users`

### Get User by ID

**GET** `/api/users/:id`

### Update User

**PUT** `/api/users/:id`

### Delete User

**DELETE** `/api/users/:id`

## API Testing

All endpoints were tested using **Bruno API Client**.

Testing Steps:

1. Create a user using POST request
2. Retrieve users using GET request
3. Retrieve a specific user by ID
4. Update the user information
5. Delete the user

Each endpoint was verified with appropriate status codes and responses.

## Status Codes Used

| Status Code | Description                   |
| ----------- | ----------------------------- |
| 200         | Successful request            |
| 201         | Resource created successfully |
| 400         | Bad request / missing fields  |
| 404         | Resource not found            |
| 500         | Internal server error         |

## Author

Developed as part of a **Backend Developer Internship Task**.
