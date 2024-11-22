
## Chat Application with OpenAI Integration and Socket.io
# Project Overview
This is a basic chat application integrated with OpenAI's GPT model to answer user questions. It allows users to:

Register and Login: Users can create accounts with encrypted passwords and log in securely.
Real-Time Messaging: Users can chat in real-time using Socket.io.
Ask Questions to GPT: Users can ask questions powered by OpenAI's GPT model.
User-Friendly Interface: The app provides simple navigation for signup, login, chatting, and asking questions.

# Technologies Used
Backend: Node.js, Express.js

Frontend: EJS, HTML, CSS

Database: MongoDB with Mongoose

Real-Time Communication: Socket.io

AI Integration: OpenAI GPT-3.5 Turbo

Password Security: Bcrypt for hashing

Environment Management: dotenv for secure API key management

# . Endpoints
GET /
Renders the login page.
GET /signup
Renders the signup page.
GET /ask
Renders the question submission page.
POST /signup
Registers a new user. Password is hashed and stored in the database.
POST /
Handles user login. Validates username and password.
POST /ask
Connects to OpenAI API and returns GPT's response for the submitted question.

# . Socket.io Events
connection: Notifies when a new user joins.
disconnect: Notifies when a user leaves.
user_message: Broadcasts user messages to all connected clients.

# How to Use
Start the server and navigate to http://localhost:port in your browser.

Sign Up: Create an account by providing a username and password.

Login: Use the registered credentials to log in.

Chat: Send and receive real-time messages.

Ask Questions: Navigate to the Ask Question page and type your query.

# Future Enhancements
Add private chat functionality.
Integrate user profiles and avatars.
Implement email verification for signup.
Enhance the UI for a more modern design.
Improve error handling and logging.
