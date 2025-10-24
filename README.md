==============================
UniVote - Voting Application
==============================

Description:
-------------
This is a backend application for a university voting system where users can vote for candidates.
It provides functionalities for user authentication, candidate management, and secure voting.

⚠️ Note: Backend Only. Use Postman or any API testing tool to interact with endpoints.

Author:
--------
Pratiyush Kumar
GitHub: https://github.com/Pratiyush-9

Features:
----------
- User sign up and login with Aadhar Card Number and password
- Users can view the list of candidates
- Users can vote for a candidate (only once)
- Admin can manage candidates (add, update, delete)
- Admin cannot vote

Technologies Used:
------------------
- Node.js
- Express.js
- MongoDB
- JSON Web Tokens (JWT) for authentication

Installation:
-------------
1. Clone the repository:
   git clone https://github.com/Pratiyush-9/UniVote-Online-Voting-System-.git

2. Navigate to the project folder:
   cd UniVote-Online-Voting-System-

3. Install dependencies:
   npm install

4. Start the development server:
   npm run dev

- The backend server will run on: http://localhost:8000
- Use Postman or any API testing tool to interact with the endpoints.

API Endpoints:
--------------

Authentication:
---------------
- Sign Up:
  POST /signup – Register a new user

- Login:
  POST /login – Login a user

Candidates:
-----------
- Get Candidates:
  GET /candidates – Retrieve the list of candidates

- Add Candidate (Admin only):
  POST /candidates – Add a new candidate

- Update Candidate (Admin only):
  PUT /candidates/:id – Update candidate by ID

- Delete Candidate (Admin only):
  DELETE /candidates/:id – Delete candidate by ID

Voting:
-------
- Get Vote Count:
  GET /candidates/vote/count – Get vote counts for all candidates

- Vote for Candidate (User only):
  POST /candidates/vote/:id – Cast vote for a candidate

User Profile:
-------------
- Get Profile:
  GET /users/profile – Get user profile information

- Change Password:
  PUT /users/profile/password – Change user password

Notes:
------
- Make sure MongoDB is running locally or provide a connection URI in a .env file.
- Admin users cannot vote.
- Each user can vote only once.

