# Real Estate Platform

A full-stack real estate web application built with Java, Spring Boot, Spring Security, PostgreSQL, Thymeleaf, and Docker.

The platform allows users to browse and search properties, manage property listings, upload property images, and access secure REST APIs with Swagger/OpenAPI documentation.

## Features

- User registration and authentication
- Role-based authorization
- Secure Spring Security implementation
- Property listing and management
- Property search and browsing
- Property details page
- User dashboard
- Admin panel
- Secure REST APIs
- PostgreSQL database integration
- Cloudinary image management
- Swagger/OpenAPI documentation
- Docker support
- Responsive web interface

## Tech Stack

### Backend

- Java
- Spring Boot
- Spring Security
- Spring Data JPA
- Hibernate
- Maven

### Database

- PostgreSQL

### Frontend

- HTML
- CSS
- JavaScript
- Thymeleaf

### Tools & Services

- Docker
- Cloudinary
- Swagger / OpenAPI
- Git
- GitHub

## Project Structure

```text
real-estate-platform/
│
├── .mvn/
│   └── wrapper/
│
├── screenshots/
│   ├── HomePage.PNG
│   ├── Listings.PNG
│   ├── PropertyDetails.PNG
│   ├── AddProperty.PNG
│   ├── UserDashboard.PNG
│   ├── AdminPanel.PNG
│   └── Swagger-ui.PNG
│
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── ...
│   │   │
│   │   └── resources/
│   │       ├── static/
│   │       ├── templates/
│   │       └── application.properties
│   │
│   └── test/
│
├── Dockerfile
├── .gitignore
├── mvnw
├── mvnw.cmd
├── pom.xml
└── README.md
```

## How to Run

### Prerequisites

Make sure you have the following installed:

- Java
- PostgreSQL
- Git
- Docker (optional)

Maven does not need to be installed separately because this project includes the Maven Wrapper.

### 1. Clone the Repository

```bash
git clone https://github.com/Thamizhmaran-k/real-estate-platform.git
cd real-estate-platform
```

### 2. Create a PostgreSQL Database

Create a PostgreSQL database for the application.

For example:

```sql
CREATE DATABASE real_estate;
```

### 3. Configure Environment Variables

The application uses environment variables for the server port, PostgreSQL database, and Cloudinary configuration.

Set the following environment variables:

```text
PORT=8080

DB_URL=jdbc:postgresql://localhost:5432/real_estate
DB_USERNAME=your_postgresql_username
DB_PASSWORD=your_postgresql_password

CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret
```

> Do not commit real passwords, API keys, or secrets to GitHub.

### 4. Set Environment Variables

#### Windows Command Prompt

```cmd
set PORT=8080
set DB_URL=jdbc:postgresql://localhost:5432/real_estate
set DB_USERNAME=your_postgresql_username
set DB_PASSWORD=your_postgresql_password
set CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
set CLOUDINARY_API_KEY=your_cloudinary_api_key
set CLOUDINARY_API_SECRET=your_cloudinary_api_secret
```

#### Windows PowerShell

```powershell
$env:PORT="8080"
$env:DB_URL="jdbc:postgresql://localhost:5432/real_estate"
$env:DB_USERNAME="your_postgresql_username"
$env:DB_PASSWORD="your_postgresql_password"
$env:CLOUDINARY_CLOUD_NAME="your_cloudinary_cloud_name"
$env:CLOUDINARY_API_KEY="your_cloudinary_api_key"
$env:CLOUDINARY_API_SECRET="your_cloudinary_api_secret"
```

### 5. Build the Project

#### Windows

```bash
mvnw.cmd clean install
```

#### Linux / macOS

```bash
./mvnw clean install
```

### 6. Run the Application

#### Windows

```bash
mvnw.cmd spring-boot:run
```

#### Linux / macOS

```bash
./mvnw spring-boot:run
```

### 7. Open the Application

Once the application starts successfully, open:

```text
http://localhost:8080
```

The application uses port `8080` by default when the `PORT` environment variable is not provided.

## API Documentation

Swagger UI is available when the application is running:

```text
http://localhost:8080/swagger-ui.html
```

The OpenAPI API documentation is available at:

```text
http://localhost:8080/v3/api-docs
```

## Docker

The project includes Docker support.

### Build the Docker Image

```bash
docker build -t real-estate-platform .
```

### Run the Docker Container

```bash
docker run -p 8080:8080 real-estate-platform
```

When running with Docker, provide the required database and Cloudinary environment variables to the container.

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

## Security

The application uses Spring Security to provide authentication and role-based authorization for protected features and application functionality.

Sensitive configuration values, including database credentials and Cloudinary API credentials, are loaded through environment variables and are not stored directly in the source code.

## Author

**Thamizhmaran K**

GitHub: https://github.com/Thamizhmaran-k
