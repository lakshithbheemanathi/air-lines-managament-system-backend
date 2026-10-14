# SkyWings Airline Management System - Backend API

Modern airline reservation and flight operations management REST API built with Java 21 LTS, Spring Boot 3, and MySQL.

## Tech Stack
- **Language**: Java 21 LTS
- **Framework**: Spring Boot 3.3.4
- **ORM / JPA**: Hibernate 6 / Spring Data JPA
- **Database**: MySQL 8+ / Aiven Cloud MySQL
- **Security**: Spring Security 6 with Stateless JWT Authentication
- **Build Tool**: Maven

## Quick Start (Local Development)

### 1. Prerequisites
- JDK 21 installed (`java -version`)
- Maven 3.9+ installed (`mvn -version`)

### 2. Configure Environment
Copy `.env.example` to `.env` or set environment variables:
```bash
cp .env.example .env
```

### 3. Run Application
```bash
mvn spring-boot:run
```
The server will start at `http://localhost:8081` (or port specified in `$PORT`).

### 4. Health Check
```bash
curl http://localhost:8081/api/health
```

## Deployment (Render Web Service)
This repository includes a multi-stage `Dockerfile` configured for zero-configuration containerized deployment on Render.
- **Runtime**: Docker
- **Environment Variables**: See `.env.example`
