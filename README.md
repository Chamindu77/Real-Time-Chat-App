
# Real-Time Chat Application

<img src="https://github.com/Vindyani1999/My-React-Projects/assets/145743416/bd6daa98-7e6a-4a2e-a1ad-f4ffe056b0cd" width="1000" height="300"/><br>
<br/>
This project is a real-time chat application built using MERN, TailwindCSS, Daisy UI, and Socket.io. It provides basic user authentication, real-time messaging, and a simple chat interface. Optional features include message notification sound, online user indication with a green dot, message persistence, and database attck managment.

## Table of Contents

1. [Setup Instructions](#setup-instructions)
2. [Application Structure](#application-structure)
3. [Features](#features)
4. [Assumptions and Limitations](#assumptions-and-limitations)
5. [Optional Features](#optional-features)
6. [Live Demo](#live-demo)

## Setup Instructions

### Prerequisites

- Node.js (v14 or later)
- npm (v6 or later)
- MongoDB (for message persistence)

### Installation

1. **Clone the repository:**

    ```bash
    git clone https://github.com/yourusername/realtime-chat-app.git
    cd realtime-chat-app
    ```

2. **Install backend dependencies:**

    ```bash
    cd backend
    npm install
    ```

3. **Install frontend dependencies:**

    ```bash
    cd ../frontend
    npm install
    ```

4. **Run the backend:**

    ```bash
    cd ../backend
    npm start
    ```

5. **Run the frontend:**

    ```bash
    cd ../frontend
    npm run dev
    ```

6. **Open the application in your browser:**

    ```
    http://localhost:3000
    ```

## Application Structure

- **backend/**

  - `controllers/`: Controller logic for handling requests.
  - `db/`: Database configuration and connection.
  - `middleware/`: Middleware functions for handling authentication and other processes.
  - `models/`: MongoDB models for storing chat data.
  - `routes/`: Express routes for handling HTTP requests.
  - `socket/`: Socket.io configuration and event handling.
  - `utils/`: Utility functions.

- **frontend/**

  - `src/`

    - `assets/`: Static assets like images and styles.
    - `components/`: React components for the chat interface.
    - `context/`: Context API for state management.
    - `hooks/`: Custom React hooks.
    - `pages/`: Page components.
    - `utils/`: Utility functions.
    - `zustand/`: State management using Zustand.

## Features

### User Authentication

- Simple user login with a username.
  ![WhatsApp Image 2024-06-01 at 12 17 57 PM](https://github.com/Vindyani1999/My-React-Projects/assets/145743416/270e242a-bf69-4488-ac6d-a9754da51dc0)


### Chat Interface

- Basic front-end interface to display messages.
- Styled with TailwindCSS.

### Real-Time Messaging

- Users can send and receive messages in real-time using Socket.io.
  ![WhatsApp Image 2024-06-01 at 12 01 46 PM](https://github.com/Vindyani1999/My-React-Projects/assets/145743416/64b28216-a242-4fdd-87cf-5d026ce9e478)

## Assumptions and Limitations

- The application is designed for demonstration purposes and may not be suitable for production without additional security and scalability considerations.

## Optional Features

### Message Notification Sound

- Users receive a notification sound when a new message is received.

### Online User Indication

- Online users are indicated with a green dot.

### Message Persistence

- Chat history is stored in MongoDB.
    - User History
     ![WhatsApp Image 2024-06-01 at 12 08 54 PM](https://github.com/Vindyani1999/My-React-Projects/assets/145743416/fd2d01fb-2b23-4151-ad6d-cc033011805a)

    - Message History
      ![WhatsApp Image 2024-06-01 at 12 09 51 PM](https://github.com/Vindyani1999/My-React-Projects/assets/145743416/bf7ab627-ea7d-4d63-b8d1-3563e9df0abf)
 
    - Conversation History
       ![WhatsApp Image 2024-06-01 at 12 10 47 PM](https://github.com/Vindyani1999/My-React-Projects/assets/145743416/2a2c328d-d690-490f-b0d6-4f01dceb32c1)

 

### Database Attck Managment

- Cross-Site Scripting(XSS) and Cross-site Request Forgery(CSRF) are used as potential database attack vectors that could be relevent in the context of using JWT and managing user session.

## Live Demo

- Demo Link:- https://real-time-chat-app-ehdj.onrender.com/login 

![Screenshot 2024-06-01 141204](https://github.com/Chamindu77/Real-Time-Chat-App/assets/117502200/285c7849-6a07-4e1f-9328-9a8ce6ff66fd)

