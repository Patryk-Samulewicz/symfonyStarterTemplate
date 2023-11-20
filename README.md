# Symfony Docker Template

## Overview

This repository contains a Symfony project set up with Docker, including a PHP environment, an Nginx web server, and a PostgreSQL database. It's configured for easy start creating apps with Symfony in Docker.

## Structure

- `project/`: Source code of the Symfony application.
- `docker/`: Docker configurations for different services.
    - `php/`: Dockerfile for the PHP environment.
    - `nginx/`: Configuration for the Nginx server.
- `docker-compose.yml`: Docker Compose configuration for running the services.

## Requirements

- Docker
- Docker Compose

## Getting Started

To get the application running, follow these steps:

### 1. Clone the Repository

```bash
git clone https://github.com/Patryk-Samulewicz/symfonyStarterTemplate.git
cd symfonyStarterTemplate
```

### 2. Run Docker Compose

```bash
docker-compose up -d --build
```

### 3. Install Dependencies (you have to install composer on your machine)

```bash
cd project
composer install
```

### 4. Open the Application

Open the application in your browser: [http://localhost:81](http://localhost:81)

### 5. Connect to the Database

- Host: `localhost`
- Port: `5432`
- Username: `main`
- Password: `main`
- Database: `DataB`


## Additional Information
- If you don't want to use the default port 81, you can change it in the `docker-compose.yml` file.
- If you don`t have symfony cli installed on your machine, you can use the following command to run symfony commands:

```bash
docker-compose exec php bin/console [command]
```
