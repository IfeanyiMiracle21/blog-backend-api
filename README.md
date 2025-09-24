Blog Backend API
A simple RESTful API for a blog platform with user authentication and CRUD operations for posts.
Setup

Clone the repository:git clone <your-repo-url>
cd blog-backend


Create and activate a virtual environment:python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate


Install dependencies:pip install -r requirements.txt


Run the server:uvicorn app.main:app --reload


Open http://127.0.0.1:8000/docs to test the API.

Endpoints

POST /users/: Create a new user (e.g., {"username": "test", "password": "pass"}).
POST /token: Login to get a JWT token.
GET /posts/: List all posts.
POST /posts/: Create a post (requires token).
GET /posts/{id}: Get a specific post.
PUT /posts/{id}: Update a post (requires token, must be post owner).
DELETE /posts/{id}: Delete a post (requires token, must be post owner).

License
MIT

## Milestone
Completed on 24/09/2025 at 01:18 PM WAT as part of my 10-day GitHub streak!