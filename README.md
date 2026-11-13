# RideLink-Driver-Vehicle-Service-
Driver and Vehicle Management Microservice - Academic Group Project

# RideLink – Driver & Vehicle Service

A Spring Boot microservice developed as part of the RideLink ride-sharing platform. This service manages driver and vehicle-related information through RESTful APIs.

## Technologies Used

- Java
- Spring Boot
- Spring Security
- MongoDB
- JWT Authentication
- Swagger / OpenAPI
- Maven
- Git & GitHub

## Features

- Driver management
- Vehicle management
- RESTful API endpoints
- MongoDB database integration
- JWT-based security support
- API documentation using Swagger
- Application health monitoring using Spring Boot Actuator

## Project Structure

```text
src/
 ├── main/
 │    ├── java/com/ridelink/driver_service/
 │    │    ├── config/
 │    │    ├── controller/
 │    │    ├── model/
 │    │    ├── repository/
 │    │    ├── security/
 │    │    └── service/
 │    └── resources/
 │         └── application.properties
 └── test/
      └── java/
```

## Configuration

Configure the MongoDB connection using an environment variable.

```properties
server.port=8082
spring.application.name=driver-vehicle-service
spring.data.mongodb.uri=${MONGODB_URI}
```

Set the MongoDB connection URI in your environment before running the application.

## Run Locally

1. Clone the repository.
2. Configure the `MONGODB_URI` environment variable.
3. Open a terminal in the project directory.
4. Run:

```bash
./mvnw spring-boot:run
```

For Windows PowerShell:

```powershell
.\mvnw.cmd spring-boot:run
```

The application runs on:

`http://localhost:8082`

## API Documentation

Swagger UI:

`http://localhost:8082/swagger-ui/index.html`

## Health Check

`http://localhost:8082/actuator/health`

## Developer

Developed as an academic microservice project for the RideLink ride-sharing platform.