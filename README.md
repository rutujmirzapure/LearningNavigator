# LearningNavigator
The exam registration service is a critical component of a Learning Management System. Generally, exam registration requires thorough Authentication and Authorization. For this assessment, your task is to develop a simplified version of the exam registration service that meets the specified requirements below.
# LMS Exam Registration System

## Description

This is a Spring Boot RESTful API application for managing exam registration in a Learning Management System (LMS). 

## Features

- **Student Management:** CRUD operations for students (create, read, update, delete).
- **Subject Management:** CRUD operations for subjects.
- **Exam Management:**  CRUD operations for exams.
- **Exam Registration:**  Register students for exams, including validation to ensure they are enrolled in the corresponding subject. 

## API Endpoints

| HTTP Method | Endpoint                       | Description                                        |
|-------------|--------------------------------|----------------------------------------------------|
| GET         | `/students`                    | Get all students                                    |
| GET         | `/students/{studentId}`         | Get a student by ID                                |
| POST        | `/students`                    | Create a new student                               |
| PUT         | `/students/{studentId}`         | Update a student by ID                                |
| DELETE      | `/students/{studentId}`         | Delete a student by ID                                |
|             |                                |                                                    |
| GET         | `/subjects`                    | Get all subjects                                    |
| GET         | `/subjects/{subjectId}`         | Get a subject by ID                                |
| POST        | `/subjects`                    | Create a new subject                               |
| PUT         | `/subjects/{subjectId}`         | Update a subject by ID                                |
| DELETE      | `/subjects/{subjectId}`         | Delete a subject by ID                                |
|             |                                |                                                    |
| GET         | `/exams`                       | Get all exams                                       |
| GET         | `/exams/{examId}`            | Get an exam by ID                                 |
| POST        | `/exams`                       | Create a new exam                                |
| PUT         | `/exams/{examId}`            | Update an exam by ID                                 |
| DELETE      | `/exams/{examId}`            | Delete an exam by ID                                 |
| POST        | `/exams/{examId}/students/{studentId}` | Register a student for an exam                    |

## How to Run

1. **Prerequisites:**
   - Java 17 or higher
   - MySQL
   - Maven (or your preferred build tool) 

2. **Clone the repository:**

   ```bash
   git clone https://github.com/<your-github-username>/<your-repository-name>.git
Use code with caution.
Markdown
Configure Database Settings:
Update the spring.datasource properties in the application.properties file with your MySQL credentials.
Run the application:
./mvnw spring-boot:run
