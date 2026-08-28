# Real Estate Platform

A full-stack real estate web application built with Java, Spring Boot, Spring Security, MySQL, and Docker.

## Features

- User authentication and authorization
- Property listing and management
- Property search and browsing
- Secure backend APIs
- MySQL database integration
- Docker support

## Tech Stack

- Java
- Spring Boot
- Spring Security
- MySQL
- HTML
- CSS
- Docker
- Maven

## Project Structure

```text
src/
├── main/
│   ├── java/
│   └── resources/
└── test/
```

## How to Run

### Prerequisites

- Java
- Maven
- MySQL
- Docker (optional)

### Local Setup

1. Clone the repository:

```bash
git clone https://github.com/Thamizhmaran-k/real-estate-platform.git
cd real-estate-platform
```

2. Configure the MySQL database and update the application configuration with your database credentials.

3. Build the project:

```bash
mvn clean install
```

4. Run the application:

```bash
mvn spring-boot:run
```

5. Open the application in your browser using the configured port.

### Docker

The project includes a Dockerfile for containerized deployment.

Build the Docker image:

```bash
docker build -t real-estate-platform .
```

Run the container:

```bash
docker run -p 8080:8080 real-estate-platform
```

## API Documentation

Swagger/OpenAPI documentation is included for exploring and testing the REST APIs.

When running locally, open:

```text
http://localhost:8080/swagger-ui/index.html
```

## Screenshots

### Home Page

![Home Page](screenshots/HomePage.PNG)

### Property Listings

![Property Listings](screenshots/Listings.PNG)

### Property Details

![Property Details](screenshots/PropertyDetails.PNG)

### Add Property

![Add Property](screenshots/AddProperty.PNG)

### User Dashboard

![User Dashboard](screenshots/UserDashboard.PNG)

### Admin Panel

![Admin Panel](screenshots/AdminPanel.PNG)

### Swagger API

![Swagger API](screenshots/Swagger-ui.PNG)
