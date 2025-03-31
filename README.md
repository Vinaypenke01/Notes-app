# Notes-app
📌 Notes App Backend (Django + DRF + MySQL) - Overview This backend-only project allows users to register, log in, and manage notes using RESTful APIs. The app is built with Django Rest Framework (DRF) and uses JWT authentication for security. The data is stored in a MySQL database.
🔹 Features
✅ User Authentication

Custom user model (Email-based login)

JWT-based authentication (Login returns a token)

✅ Notes Management

Create Notes

Retrieve Notes

Update Notes

Delete Notes

✅ Database

Uses MySQL for storing users and notes

✅ API Endpoints

Method	Endpoint	Description
POST	/api/register/	Register a new user
POST	/api/login/	Log in & get JWT token
GET	/api/notes/	Get all notes for logged-in user
POST	/api/notes/	Create a new note
PUT	/api/notes/<id>/	Update a note
DELETE	/api/notes/<id>/	Delete a note
🔹 Technologies Used
Backend Framework: Django, Django REST Framework

Database: MySQL

Authentication: JWT (JSON Web Token)

API Testing: Postman

🔹 How It Works
User Registration

A user registers using an email, username, and password.

The password is securely hashed before storing it in MySQL.

User Login

The user logs in using email and password.

If correct, a JWT token is issued, which is required for further API access.

Notes Management

Only authenticated users can create, update, delete, and retrieve their notes.

Each note is linked to a specific user, ensuring data privacy.
