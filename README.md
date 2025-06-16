Real-Time Chat App with Golang, Angular, and WebSocket
This project is a real-time chat application built using Golang on the backend, Angular 2+ on the frontend, and WebSocket for bidirectional communication.

Features
Real-time messaging between multiple users

WebSocket-based communication for low-latency updates

Angular standalone components with modern best practices

Simple and clean UI for chat interaction

Automatic connection open/close handling

Technologies Used
Backend: Golang (net/http, Gorilla WebSocket, or native websocket libraries)

Frontend: Angular 2+ (standalone components, bootstrapApplication)

Communication: WebSocket protocol for real-time message exchange

Prerequisites
Go installed (1.16+ recommended)

Node.js and npm installed

Angular CLI (npm install -g @angular/cli) or use npx

Setup and Installation
Backend (Golang)
Navigate to the backend folder (e.g., backend/):

bash
Copy
Edit
cd backend
Run the Go WebSocket server:

bash
Copy
Edit
go run main.go
The WebSocket server will start listening on ws://localhost:12345/ws

Frontend (Angular)
Navigate to the frontend folder (e.g., frontend/):

bash
Copy
Edit
cd frontend
Install dependencies:

bash
Copy
Edit
npm install
Run the Angular development server:

bash
Copy
Edit
ng serve --open
This will open the app in your default browser at http://localhost:4200.

Usage
Type messages into the input box at the bottom of the screen.

Press Send or hit Enter to send a message.

Messages from all connected clients will appear in real-time.

Project Structure
bash
Copy
Edit
/
├── backend/              # Golang WebSocket server
│   └── main.go
├── frontend/             # Angular application
│   ├── src/
│   ├── angular.json
│   ├── package.json
│   └── ...
└── README.md
Notes
Make sure the backend server is running before starting the Angular frontend.

Adjust WebSocket URL in SocketService if backend runs on a different host or port.

This project uses Angular standalone components and the new bootstrapApplication API.