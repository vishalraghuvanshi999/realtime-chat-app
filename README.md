# realtime-chat-app
# Real-Time Chat Application

A full-stack real-time messaging application that enables users to communicate instantly through WebSockets. The project demonstrates how modern messaging platforms handle authentication, real-time communication, and persistent message storage.

---

## Features

* User registration and login
* Secure authentication using JSON Web Tokens (JWT)
* Real-time messaging with WebSockets
* Persistent chat history
* Online/offline user status
* Responsive user interface

---

## Tech Stack

### Frontend

* React.js
* Axios
* Tailwind CSS

### Backend

* Node.js
* Express.js
* Socket.io

### Database

* MongoDB

---

## Architecture

```
Client (React)
      |
      | REST API
      v
Node.js + Express Server
      |
      | WebSocket (Socket.io)
      v
MongoDB Database
```

The application uses REST APIs for authentication and data management, while Socket.io handles real-time message delivery between connected users.

---

## Project Structure

```
realtime-chat-app
│
├── backend
│   ├── controllers
│   ├── models
│   ├── routes
│   ├── socket
│   └── server.js
│
├── frontend
│   ├── components
│   ├── pages
│   ├── services
│   └── App.js
│
└── README.md
```

---

## Installation

### Clone the repository

```
git clone https://github.com/vishalraghuvanshi999/realtime-chat-app.git
cd realtime-chat-app
```

### Backend Setup

```
cd backend
npm install
npm start
```

### Frontend Setup

```
cd frontend
npm install
npm start
```

---

## Environment Variables

Create a `.env` file inside the backend directory.

```
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
```

---

## Future Improvements

* Group chat functionality
* File sharing
* Typing indicators
* Message read receipts
* Push notifications

---

## License

This project is available under the MIT License.

