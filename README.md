# Chronotimer Project

!flow diagram

## Overview

Chronotimer is a comprehensive time management application built using Spring Boot, Microservices, SQL, and React. It allows users to manage their time entries, projects, and remarks efficiently. The application is designed with a microservices architecture, ensuring scalability and maintainability.

## Features

### User Management
- **Register**: Create a new user account.
- **Authenticate**: User login with JWT authentication.
- **Fetch All Employees**: Retrieve a list of all employees.
- **Remove**: Delete a user account.
- **Edit Details**: Update user information.

### Timer Management
- **Add Time Entry**: Log a new time entry.
- **Edit Time Entry**: Modify an existing time entry.
- **Delete Time Entry**: Remove a time entry.
- **Get All Time Entries**: Retrieve all time entries.
- **Approved Hours (Monthly View)**: View approved hours in a monthly format.
- **Detailed Daily Timesheet**: View detailed daily timesheets.

### Project Management
- **Get Project By ID**: Retrieve project details by ID.
- **Add Project**: Create a new project.
- **Delete Project**: Remove a project.
- **Edit Project**: Update project details.
- **Get All Projects**: Retrieve a list of all projects.

### Remarks Management
- **Add Remark**: Add a new remark.
- **Get Remarks by ID**: Retrieve remarks by ID.
- **Delete Remarks by ID**: Remove remarks by ID.

## Architecture

The application is built using a microservices architecture, with the following components:

- **APIGateway**: Acts as the entry point for all client requests.
- **EurekaServer**: Service registry for managing microservices.
- **Config Server**: Centralized configuration management.
- **Security Service**: Manages user authentication and authorization.
- **Timer Service**: Handles time entry operations.
- **Project Service**: Manages project-related operations.
- **Remarks Service**: Handles remark-related operations.
- **React**: Frontend application for user interaction.

## Database

The application uses SQL databases for storing data related to users, time entries, projects, and remarks. Each microservice has its own dedicated database to ensure data isolation and integrity.

## Getting Started

### Prerequisites

- Java 11 or higher
- Node.js and npm
- MySQL or any other SQL database

### Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/p-amrithnath/Chronotimer-Project.git
   cd Chronotimer-Project
Set up the backend services:

cd Chronotimer_Backend
./mvnw clean install
./mvnw spring-boot:run
Set up the frontend application:

cd Chronotimer_Frontend
npm install
npm start
Configuration
Update the database configuration in the application.properties files for each microservice.
Configure the Config Server with the necessary properties for each service.
Contributing
Contributions are welcome! Please fork the repository and create a pull request with your changes.

License
This project is licensed under the MIT License. See the LICENSE file for details.

Acknowledgements
Spring Boot
React
MySQL
Bootstrap
