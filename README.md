This Spring Boot-based Task Manager application provides a RESTful API for managing tasks and notes. It allows users to add tasks with customizable due dates (defaulting to 7 days ahead), update task details (due date, status), delete tasks, and manage associated notes. Notes can be added, viewed, or deleted for specific tasks. The project uses Gradle for dependency management and H2 as the embedded database, ensuring lightweight and rapid development. API endpoints include operations for tasks (GET, POST, PATCH, DELETE) and notes associated with tasks. The application can be run via gradle bootRun or ./gradlew bootRun. Docker support is also available for containerized deployment.


![image](https://github.com/user-attachments/assets/0f7b10cd-8c30-4986-b912-11f953da499f)
