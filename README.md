# Task Manager + Notes Support

## Overview
- A simple task manager application with RESTful APIs for managing tasks and their associated notes.
- Allows users to create, update, delete tasks, and attach notes to specific tasks.

## Features
- Add new tasks with a customizable due date (default is 7 days from today).
- Update task details (due date, status: done/not done).
- Delete tasks when no longer needed.
- Manage notes associated with tasks:
  - Add notes to tasks.
  - View all notes for a task.
  - Delete specific notes.

## API Endpoints
### Task Management
- **GET /tasks**: Retrieve all tasks.
- **GET /tasks/{id}**: Retrieve a specific task by ID.
- **POST /tasks**: Create a new task.
- **PATCH /tasks/{id}**: Update an existing task (status, due date, or name).
- **DELETE /tasks/{id}**: Delete a specific task.

### Notes Management
- **GET /tasks/{id}/notes**: Retrieve all notes associated with a specific task.
- **POST /tasks/{id}/notes**: Add a new note to a task.
- **DELETE /tasks/{id}/notes/{nid}**: Delete a specific note from a task.

## Database Schema
### Tasks Table
- **id**: int, primary key
- **name**: string, task name
- **due_date**: date, task deadline
- **status**: boolean, task completion status (done/not done)

### Notes Table
- **id**: int, primary key
- **body**: string, note content
- **task_id**: int, foreign key referencing tasks.id

## Key Concepts
- **Idempotency**: Ensures that repeated requests (e.g., DELETE) have the same effect.
- RESTful design principles for API development.



![image](https://github.com/user-attachments/assets/0f7b10cd-8c30-4986-b912-11f953da499f)
