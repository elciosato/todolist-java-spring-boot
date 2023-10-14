# TodoList Project
## Project Overview

This project, developed using the Spring Boot framework, exemplifies the power and versatility of the Java language.

It is a straightforward API designed for a Todo List application, making it a valuable resource for gaining insights into real-world project development. This project can serve as a reference for those looking to explore Java-based API development.

## Endpoints
### Create User
```bash
# POST - http://localhost:8080/users/
# BODY
{
	"username": "johndoe",
	"name": "John Doe",
	"password": "123456"
}
```
### Create Task
Need a basic authentication, username and password
```bash
# POST - http://localhost:8080/tasks/
# BODY
{
	"title": "Try this project",
	"description": "Try this awesome project",
	"priority": "HIGH",
	"startAt": "2023-10-15T10:00:00",
	"endAt": "2023-10-15T12:00:00"
}
```
### List Tasks
Need a basic authentication, username and password
```bash
# GET - http://localhost:8080/tasks/
# Result
[
	{
		"id": "aa2df27b-a709-4883-b937-e63d49267258",
		"description": "Try this awesome project",
		"title": "Try this project",
		"startAt": "2023-10-15T10:00:00",
		"endAt": "2023-10-15T12:00:00",
		"priority": "HIGH",
		"createdAt": "2023-10-14T13:06:03.774",
		"userId": "9b882973-56fd-473c-8eb4-cf3012e87cc3"
	}
]
```
### Update Task
Need a basic authentication, username and password
```bash
# PUT - http://localhost:8080/tasks/{id}
# BODY
{
	"title": "Trying this project",
	"description": "Trying this awesome project"
}
```