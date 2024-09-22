# Django HTMX Docker Project

This project is a Django application using HTMX, containerized with Docker and orchestrated with Docker Compose.

## Prerequisites

- Docker
- Docker Compose

## Setup

1. Clone the repository:
   ```
   git clone <repository-url>
   cd <project-directory>
   ```

2. Create a `.env` file in the root directory with the following variables:
   ```
   POSTGRES_DB=your_db_name
   POSTGRES_USER=your_db_user
   POSTGRES_PASSWORD=your_db_password
   DB_HOST=db
   DB_PORT=5432
   ```
   Replace the values with your preferred database settings.

3. Build the Docker images:
   ```
   docker-compose build
   ```

## Running the Application

1. Start the containers:
   ```
   docker-compose up
   ```

2. The application will be available at `http://localhost:8000`

3. To run in detached mode:
   ```
   docker-compose up -d
   ```

## Database Migrations

To run database migrations:
