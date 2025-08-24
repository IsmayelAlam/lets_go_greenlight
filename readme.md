# Let's Go Further — Practice Project

This repository contains my practice and follow-along project for the book **"Let's Go Further" by Alex Edwards**. The goal of this project is to deepen my understanding of Go web application development by implementing the concepts, examples, and exercises presented in the book.

## About the Book

["Let's Go Further"](https://lets-go-further.alexedwards.net/) is the sequel to _Let's Go_, focusing on advanced topics in Go web development. It covers areas such as:

- Authentication and authorization
- Middleware
- Security best practices
- Structuring and organizing large projects
- Background tasks and worker processes
- File uploads and downloads
- Advanced testing strategies

## Project Goals

- Reinforce concepts by coding along with the book.
- Experiment with variations and custom implementations.
- Build a working Go web application that incorporates advanced features and best practices.
- Document progress and insights for future reference.

## Requirements

- **Go 1.24+**
- A code editor (e.g., VS Code, GoLand)
- Basic understanding of Go (functions, structs, interfaces, etc.)
- Familiarity with the _Let's Go_ book or basic Go web development

## Repository Structure

```
.
├── cmd/            # Application entry points
│   └── api/        # Web application
├── internal/       # Core application code
│   ├── data/       # Data models
│   ├── validator/  # Form validation helpers
│   ├── mailer/     # Sending emails
│   └── vcs/        # version
├── migrations/     # Database migrations
├── remote/         # Deployment
├── go.mod          # Module definition
└── go.sum          # Dependency checksums
```

## Endpoint

| Method | URL Pattern               | Action                                          |
| ------ | ------------------------- | ----------------------------------------------- |
| GET    | /v1/healthcheck           | Show application health and version information |
| GET    | /v1/movies                | Show the details of all movies                  |
| POST   | /v1/movies                | Create a new movie                              |
| GET    | /v1/movies/:id            | Show the details of a specific movie            |
| PATCH  | /v1/movies/:id            | Update the details of a specific movie          |
| DELETE | /v1/movies/:id            | Delete a specific movie                         |
| POST   | /v1/users                 | Register a new user                             |
| PUT    | /v1/users/activated       | Activate a specific user                        |
| PUT    | /v1/users/password        | Update the password for a specific user         |
| POST   | /v1/tokens/authentication | Generate a new authentication token             |
| POST   | /v1/tokens/password-reset | Generate a new password-reset token             |
| GET    | /debug/vars               | Display application metrics                     |

---

📚 This project is for learning and practice purposes only. It closely follows the structure and examples from _Let's Go Further_.

<!-- docker run --name postgres -p 5432:5432 -e POSTGRES_PASSWORD=postgres -d postgres -->
