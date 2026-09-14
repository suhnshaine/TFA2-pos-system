# TFA2 - From Arrays to a Real Database (CodeIgniter POS)

## Overview

This project is a continuation of the Point-of-Sale (POS) system developed in TFA1 using CodeIgniter 4. The application follows the Model-View-Controller (MVC) architecture and replaces the static PHP arrays from the previous activity with a MySQL database. Customer and user data are retrieved through CodeIgniter Models using Query Builder methods.

## Features

- Landing Page
- About Page
- Customer Accounts Page
- User Accounts Page
- MySQL Database Integration
- CodeIgniter Models
- Query Builder Data Retrieval
- MVC Architecture

## Technologies Used

- PHP
- CodeIgniter 4
- MySQL
- XAMPP
- Composer
- HTML/CSS

## Installation

### Clone the Repository

```bash
git clone https://github.com/suhnshaine/TFA2-pos-system.git
```

### Navigate to the Project Folder

```bash
cd TFA2-POS-System
```

### Install Dependencies

```bash
composer install
```

## Database Setup

1. Create a database named:

```text
pos_system
```

2. Import the database export file:

```text
database/pos_system.sql
```

3. Ensure Apache and MySQL are running in XAMPP.

## Environment Configuration

Rename the provided environment file:

```text
env -> .env
```

Configure the database connection:

```ini
database.default.hostname = localhost
database.default.database = pos_system
database.default.username = root
database.default.password =
database.default.DBDriver = MySQLi
database.default.port = 3306
```

Configure the application URL:

```ini
app.baseURL = 'http://localhost:8080/'
```

## Running the Application

Start the development server:

```bash
php spark serve
```

Open:

```text
http://localhost:8080
```

## Available Pages

| Route | Description |
|---------|-------------|
| / | Landing Page |
| /about | About Page |
| /customers | Customer Accounts |
| /users | User Accounts |

## MVC Implementation

The application follows the Model-View-Controller (MVC) architecture.

- Routes map incoming URL requests to controller methods.
- Controllers handle requests and retrieve data through Models.
- Models communicate with the MySQL database using Query Builder methods such as `findAll()`.
- Views receive data from controllers and display the results to users.

## Database Tables

### Customers

- id
- full_name
- email
- phone
- created_at

### Users

- id
- username
- full_name
- created_at

## Live Demo

NOT YET HOSTED

## Author

**SHIREALETH ACORDA**

FEU Institute of Technology
