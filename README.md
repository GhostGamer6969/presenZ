# presenZ: College Management System

## Overview
presenZ is a web-based application built with Python Django and SQLite3, designed to streamline administrative and academic operations for colleges. It uses Bootstrap for the frontend to provide a responsive and user-friendly interface. Additionally, the system is available as a Docker container for easy deployment.

## Features
- **Student Management**: Add, update, and delete student details.
- **Faculty Management**: Manage faculty records and assignments.
- **Course Management**: Create and manage courses and schedules.
- **Attendance Tracking**: Record and track attendance for students.
- **Dashboard**: Intuitive dashboard for administrators with key metrics and insights.

## Tech Stack
- **Backend**: Python (Django Framework)
- **Database**: SQLite3
- **Frontend**: Bootstrap
- **Deployment**: Docker

## Installation

### Prerequisites
- Python 3.7+
- Docker (optional, for containerized deployment)

### Steps to Run Locally
1. Clone the repository:
   ```bash
   git clone https://github.com/GhostGamer6969/presenZ.git
   cd presenZ
   ```

2. Install the dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Apply database migrations:
   ```bash
   python manage.py migrate
   ```

4. Start the development server:
   ```bash
   python manage.py runserver
   ```
   Access the application at `http://127.0.0.1:8000/`.

### Steps to Run with Docker
1. Pull the Docker container:
   ```bash
   docker pull ghostgamer6969/ams:1.4
   ```

2. Run the Docker container:
   ```bash
   docker run -p 8000:8000 ghostgamer6969/ams:1.4
   ```
   Access the application at `http://127.0.0.1:8000/`.

## Project Structure
```
presenZ/
|— manage.py
|— requirements.txt
|— Dockerfile
|— media
  |— default
  |— images
|— static
  |— assets
|— attendance
  |— admin.py
  |— forms.py
  |— ...
|— app/
    |— migrations/
    |— templates/
    |— models.py
    |— views.py
    |— urls.py
    |— ...
```
