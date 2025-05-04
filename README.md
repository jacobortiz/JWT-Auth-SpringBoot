# JWT Authentication API with Spring Boot

A secure REST API implementation using Spring Boot and JWT (JSON Web Token) authentication.

## Features

- JWT-based authentication
- MySQL database integration
- Spring Security implementation
- RESTful API endpoints
- User registration and authentication
- Secure password handling

## Prerequisites

- Java 17 or higher
- Maven
- MySQL Server (running on port 3307)

## Configuration

The application requires the following environment setup:

1. MySQL database running on port 3307
2. Database name: `taskdb`
3. Default credentials:
   - Username: `root`
   - Password: `secret`

You can modify these settings in `src/main/resources/application.properties`.

## Installation

1. Clone the repository
2. Install dependencies:
```bash
mvn install
```

## Running the Application

To start the application:
```bash
mvn spring-boot:run
```

The server will start on port 8005.

## Security Configuration

- JWT secret key is configured in `application.properties`
- Token expiration time is set to 1 hour (3600000 milliseconds)
- Hibernate is configured to automatically update the database schema

## API Endpoints

The API provides the following endpoints:

- `/api/auth/register` - Register a new user
- `/api/auth/login` - Authenticate and get JWT token
- `/api/test/**` - Protected endpoints requiring authentication

## Development

This project uses:
- Spring Boot 3.4.5
- Spring Security
- Spring Data JPA
- MySQL Connector
- JJWT for JWT implementation

## License

This project is licensed under the MIT License.