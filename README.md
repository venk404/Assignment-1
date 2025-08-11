
# Student Management API

This project is a simple Student Management API built using FastAPI. It allows for basic CRUD operations on student data. The API supports creating, reading, updating, and deleting student information.



## Features

- Create Student: Add a new student.
- Get All Students: Retrieve a list of all students.
- Get Student by ID: Retrieve a specific student by their ID.
- Update Student: Update a student's information.
- Delete Student: Delete a student by their ID.


## Requirments
- Python 3.11+
- PIP
- Make
- Docker & Docker Compose(For database)
## Installation
1) Clone the repository:

```bash
  git clone https://github.com/venk404/SRE--RestAPI.git
```
2) Docker Componse for Postgres Installation:
```bash
  cd DB/Schemas
  docker-compose up -d
```
3) Execute the makeFile command (assuming make is installed on your system). This will initiate the servers and generate the student schema:

```bash
  cd ..
  make all
```

__If you don't have make, then follow the steps below:-__

2) Create a virtual environment and activate it:

```bash
  python -m venv venv
  venv\Scripts\activate.ps1
  venv\Scripts\python -m pip install --upgrade pip
```

3) Install the required packages and create schema:
```bash
  venv\Scripts\pip install -r requirements.txt
  venv\Scripts\python DB\Schemas\Create_Student.py
```

4) Come outside the folder DB and Start the server
```bash
  cd ..
  uvicorn main:app --reload
```



## Documentation(API Documentation)

- Refer to the API documentation for the endpoints listed below
```bash
  http://127.0.0.1:8000/docs
```

