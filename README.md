# Drinks API (Django REST Framework)

# Description
This project is a RESTful API built using Django and Django REST Framework for managing drink data. It supports CRUD (Create, Read, Update, Delete) operations and demonstrates API development using model serialization and structured endpoints.

---

# Project Overview
The application provides endpoints to create, retrieve, update, and delete drink records. It uses Django models to define the data structure and Django REST Framework serializers to convert model instances into JSON format.

---

# Problem Statement
Building scalable APIs requires proper structuring of models, serialization, and request handling. This project demonstrates how to design a clean REST API using Django REST Framework while maintaining separation between data models and API responses.

---

# Key Features
- Create new drinks
- Retrieve all drinks
- Retrieve a single drink by ID
- Update existing drink details
- Delete drinks
- JSON-based API responses
- Model serialization using Django REST Framework



# Tech Stack
- Backend: Django
- API Framework: Django REST Framework
- Language: Python
- Database: SQLite



# API Endpoints

## Get All Drinks
GET /drinks/

## Get Drink by ID
GET /drinks/<id>

## Create Drink
POST /drinks/

## Update Drink
PUT /drinks/<id>

## Delete Drink
DELETE /drinks/<id>

---

# Data Model

## Drink
- name: string
- description: string

---

# How It Works
The application uses Django models to define the structure of drink data. Django REST Framework serializers convert model instances into JSON and validate incoming data.

Views handle HTTP requests and return appropriate responses based on the request type (GET, POST, PUT, DELETE). Each endpoint interacts with the database through Django’s ORM.

---

# Example Usage

You can test the API using tools like Postman or a simple Python script:

```python
import requests

response = requests.get('http://127.0.0.1:8000/drinks')
print(response.json())
