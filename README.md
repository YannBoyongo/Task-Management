# Task Management System

A comprehensive full-stack task management system built with a Laravel backend, React frontend, and containerized using Docker.

## Overview

The application runs four containerized services:

- **Laravel Backend API**
- **React Frontend**
- **MySQL Database**
- **phpMyAdmin Interface**

## Features

### User Authentication
- User registration
- Secure login system
- Role-based access control

### Task Management
- Create, read, update, and delete tasks
- Task status tracking and updates
- Task assignment system

### Administrative Controls
- Admin dashboard
- User management
- Task assignment capabilities
- System-wide monitoring

### Containerized Environment
- Isolated services
- Easy deployment
- Consistent development environment

## Prerequisites

Ensure you have the following installed:
- **Docker**
- **Docker Compose**

## Installation

### Clone the Repository
```bash
git clone https://github.com/your-username/task-management-system.git
cd task-management-system
```

### Launch Services
```bash
docker-compose up --build
```

## Accessing the Application

| Service       | URL                          | Description               |
|--------------|-----------------------------|---------------------------|
| Frontend     | http://localhost:3000       | React user interface      |
| Backend API  | http://localhost:8000       | Laravel API endpoints     |
| phpMyAdmin   | http://localhost:8080       | Database management UI    |

## API Documentation

### Authentication Endpoints

| Method | Endpoint         | Description            | Access  |
|--------|-----------------|------------------------|---------|
| POST   | /api/register   | User registration      | Public  |
| POST   | /api/login      | User authentication    | Public  |

### Task Management Endpoints

| Method | Endpoint              | Description          | Access  |
|--------|----------------------|----------------------|---------|
| POST   | /api/tasks            | Create task         | Admin   |
| GET    | /api/tasks            | List all tasks      | All Users |
| GET    | /api/tasks/{id}       | Get task details    | All Users |
| PUT    | /api/tasks/{id}       | Update task         | Admin   |
| DELETE | /api/tasks/{id}       | Delete task         | Admin   |
| PATCH  | /api/tasks/{id}/status | Update task status  | All Users |

## Frontend Application

The React frontend provides:
- Intuitive user interface
- Real-time task updates
- Responsive design
- Role-based interface adaptation
- Integration with Laravel backend API

## User Interface Features

### Admin Dashboard
- Task creation and assignment
- User management
- System monitoring

### User Dashboard
- Task viewing
- Status updates
- Personal task management

---

### License
This project is licensed under the MIT License.

### Contributing
Feel free to fork the repository and submit pull requests!

