Django JWT API

A JWT-based authentication system built with Django and Django REST Framework (DRF). This project provides a secure and scalable authentication mechanism using JSON Web Tokens (JWT) for API authentication.

Features 🚀

✅ User Registration & Login

✅ JWT-based Authentication (Access & Refresh Tokens)

✅ Token Refresh Endpoint

✅ Protected Routes with Authentication

✅ Secure Logout Implementation

Tech Stack 🛠️

Django – High-level Python web framework

Django REST Framework (DRF) – Powerful API toolkit

JWT (JSON Web Token) – Secure token-based authentication

Installation & Setup

Prerequisites

Make sure you have Python 3.x and pip installed on your system.

Steps to Set Up the Project

# Clone the repository
git clone https://github.com/yourusername/django-jwt-api.git
cd django-jwt-api

# Create a virtual environment
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run migrations
python manage.py migrate

# Start the development server
python manage.py runserver

API Endpoints 📌

Authentication Endpoints

Method                       Endpoint             Description
POST                       /register/            User registration
POST                     /login/                 User login & token generation
POST                    /logout/                 Logout & token invalidation
POST                   /refreshtoken/            Refresh expired access token
GET                    /protected/               Access protected route    

Usage 🛠️

Use Postman or any API client to test endpoints.

Register a new user by sending a POST request to /register/ with { "username": "test", "password": "password" }.

Log in using /login/ to receive an access and refresh token.

Access protected routes using the provided JWT token in the Authorization header.

Refresh your access token using /refreshtoken/.

Contributing 🤝

Feel free to submit issues and pull requests! Contributions are always welcome. 😊

License 📝

This project is licensed under the MIT License.
