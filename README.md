# Flask User API

This is a simple Flask application that allows users to register and retrieve user information via API endpoints.

## Features

- Register a new user with a username and email (`POST /register`)
- Retrieve user details by username (`GET /user/<username>`)

## How to Run

1. Clone the repository:
git clone https://github.com/Priyadarshini777/flask_user_api.git

csharp
Copy
Edit
2. Navigate into the project directory:
cd flask_user_api

cpp
Copy
Edit
3. (Optional) Create and activate a virtual environment:
python -m venv venv
source venv/bin/activate # On Windows: venv\Scripts\activate

markdown
Copy
Edit
4. Install dependencies:
pip install flask

markdown
Copy
Edit
5. Run the Flask app:
python app.py

markdown
Copy
Edit
6. Open your browser or Postman and visit:
http://127.0.0.1:5000/

pgsql
Copy
Edit

## API Endpoints

- `POST /register` — Register a new user.  
**Request Body (JSON):**  
```json
{
 "username": "your_username",
 "email": "your_email@example.com"
}
GET /user/<username> — Get details of a specific user.

Notes
This project uses an in-memory dictionary to store users, so data will be lost when the app stops.

For production, consider using a proper database.
