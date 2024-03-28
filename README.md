# Ecom-Backend

## Overview
The Ecom Backend project with Sequelize ORM integration is crucial for building a robust backend system for managing data. It provides a structured and efficient way to interact with a MySQL database, offering features like schema management, data seeding, and API endpoints for CRUD operations. By using environment variables for sensitive information and leveraging Sequelize's capabilities, the project ensures secure database connections and easy maintenance.

## Table of Contents
- [Overview](#overview)
- [Getting Started](#getting-started)
- [Features](#features)
- [Contributing](#contributing)
- [Tests](#tests)
- [License](#license)
- [Questions](#questions)

## Getting Started
Watch a video demonstration of the project [here](https://youtu.be/8VO373lwoyM).

1. **Install Dependencies:**

    Make sure you have Node.js installed. Then, in your project directory, run the following command to install the required dependencies:
    ```
    npm install
    ```
2. **Create .env File:**

    Create a file named .env in your project's root directory. Add the following database configuration variables to it:
    ``` 
    DB_NAME=your_database_name
    DB_USER=your_mysql_username
    DB_PASSWORD=your_mysql_password
    ```
3. **Access MySQL Command Line:**

    Open your terminal or command prompt and enter the following command to access the MySQL command line using your root user:
    ```
    mysql -u root -p
    ```    
    You'll be prompted to enter your MySQL root password.
4. **Create and Use Database:**

    Once you're in the MySQL command line, you can create and use your database using the following commands:
    ```
    CREATE DATABASE IF NOT EXISTS database_name;
    USE database_name;
    ```
    Replace database_name with the name you specified in the .env file.
5. **Setup Schema:**

    In your project's db folder, you should have separate SQL files for (schema.sql).
    Run the following command in the MySQL command line to set up your database schema data:
    ```
    source db/schema.sql;
    ```
6. **Run Your Application:**
7. 
    Before starting your Node.js application, seed the database with initial data using the following command:
    ```
    npm run seed
    ```
    After seeding the database, you can run your Node.js application to start using it:
    ```
    npm start
    ```
    By following these steps in order, users can easily set up and start using your app with the required database configuration and initial data. Adjust the file paths and commands as per your project's structure.
<img src="assets\employee-table.png" title="Employee Table">

## Features

**Environment Variable Setup:**
- Safely store database credentials in an environment variable file for security.
**Database Connection:**
- Seamlessly connect to MySQL database using Sequelize ORM for efficient data handling.
**Schema and Seeding:**
- Initialize a development database with schema definitions and seed it with test data for testing and development purposes.
**Server Start and Sync:**
- Launch the Express server to handle API requests and automatically sync Sequelize models with the MySQL database for data consistency.
**CRUD Operations:**
- Implement API endpoints for creating, reading, updating, and deleting data (categories, products, tags) to manage database records effectively.
**Formatted JSON Responses:**
- Receive formatted JSON responses for API GET routes, making it easier to consume and display data in frontend applications.

## Contributing
Thank you for considering contributing to our project! Follow these steps:

* Fork the repository and clone it to your local machine.
* Create a branch, make your changes, and commit them with a clear message.
* Push your changes to your forked repository.
* Open a pull request on the original repository.

Guidelines
* Follow existing code style and conventions.
* Ensure your code is well-documented.

Pull Requests
* Keep them focused and provide a clear description.
* Reference relevant issues if applicable.

## Tests
**Testing Functionality with Insomnia:**
  To test the functionality of the project using Insomnia: 
  - Set up environment variables for database credentials.
  - Initialize the database with schema and seed data.
  - Start the Express server and ensure Sequelize models are synced with the database.
  - Use Insomnia to test API endpoints for CRUD operations (GET, POST, PUT, DELETE) on categories, products, and tags.
  - Verify that the project functions as expected by receiving formatted JSON responses and successfully performing data manipulation operations.
  By following these steps and leveraging Insomnia for API testing, developers can ensure the reliability and effectiveness of the Express.js API project with Sequelize integration.

## License
![None License](https://img.shields.io/badge/License-None-brightgreen)
This project is not licensed and is provided as-is without any warranty. You are free to use, modify, and distribute the code as you see fit. However, we do not provide any legal protection or support for this project.


## Questions
For questions about this project, contact [Parker Rappleye](https://github.com/prappleman) via email at parker.rappleye1@gmail.com.
