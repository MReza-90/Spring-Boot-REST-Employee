

# Employee Directory REST API

## Overview

This project provides a REST API for managing an employee directory. It allows clients to perform CRUD (Create, Read, Update, Delete) operations on employee data.

## Features

- **Get a list of employees**: Retrieve a list of all employees in the directory.
- **Get a single employee by ID**: Fetch detailed information about a specific employee by their unique ID.
- **Add a new employee**: Add a new employee to the directory.
- **Update an employee**: Modify the details of an existing employee.
- **Delete an employee**: Remove an employee from the directory.

## Getting Started

### Prerequisites

- Java 17 or higher
- Maven or Gradle (depending on your build tool)
- An IDE such as IntelliJ IDEA or Eclipse 

### Installation

1. **Clone the Repository**

   ```bash
   git clone https://github.com/MReza-90/Spring-Boot-REST-Employee.git 
   cd employee-directory-rest-api
   ```

2. **Build the Project**

   If you’re using Maven:

   ```bash
   mvn clean install
   ```

   If you’re using Gradle:

   ```bash
   ./gradlew build
   ```

3. **Run the Application**

   You can run the application using the following command:

   ```bash
   mvn spring-boot:run
   ```

   or, if you’re using Gradle:

   ```bash
   ./gradlew bootRun
   ```

   Alternatively, you can run the packaged JAR file:

   ```bash
   java -jar target/employee-directory-rest-api-0.0.1-SNAPSHOT.jar
   ```

### API Endpoints

- **Get a list of employees**

  - **URL**: `/api/employees`
  - **Method**: `GET`
  - **Response**: List of employees

- **Get a single employee by ID**

  - **URL**: `/api/employees/{employeeId}`
  - **Method**: `GET`
  - **Response**: Employee details

- **Add a new employee**

  - **URL**: `/api/employees`
  - **Method**: `POST`
  - **Request Body**: Employee data
  - **Response**: Created employee details

- **Update an employee**

  - **URL**: `/api/employees/{employeeId}`
  - **Method**: `PUT`
  - **Request Body**: Updated employee data
  - **Response**: Updated employee details

- **Delete an employee**

  - **URL**: `/api/employees/{employeeId}`
  - **Method**: `DELETE`
  - **Response**: Confirmation of deletion

### Testing

To run the tests, use:

- Maven:

  ```bash
  mvn test
  ```

- Gradle:

  ```bash
  ./gradlew test
  ```

### Configuration

Configuration settings can be found in `src/main/resources/application.properties`. Modify these settings as needed for your environment.

### Contributing

If you’d like to contribute to this project, please fork the repository and submit a pull request. For detailed contribution guidelines, see [CONTRIBUTING.md](CONTRIBUTING.md).

