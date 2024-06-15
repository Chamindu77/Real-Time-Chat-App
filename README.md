
# Real-Time Chat Application

<img src="https://github.com/Chamindu77/Real-Time-Chat-App/assets/117502200/f79036b5-e0aa-4a71-8cc0-832746d649b5" width="1000" height="300"/><br>
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

- Simple user Signup and Signin with username and password.
 ![Screenshot 2024-06-04 090527](https://github.com/Chamindu77/Real-Time-Chat-App/assets/117502200/4e9bdb91-7ec9-4679-b082-658a205f954e) 


### Chat Interface

- Basic front-end interface to display messages.
- Styled with TailwindCSS.

### Real-Time Messaging

- Users can send and receive messages in real-time using Socket.io.
  ![Screenshot 2024-06-04 090547](https://github.com/Chamindu77/Real-Time-Chat-App/assets/117502200/f044af94-89b1-4e6e-a73f-5dd9a9254541)


## Assumptions and Limitations

- The application is designed for demonstration purposes and may not be suitable for production without additional security and scalability considerations.

## Optional Features

### Message Notification Sound

- Users receive a notification sound when a new message is received.

### Online User Indication

- Online users are indicated with a green dot.
  
  ![image](https://github.com/Chamindu77/Real-Time-Chat-App/assets/117502200/053aac46-8f5c-4e1f-85f6-33338d48df5f)


### Message Persistence

- Chat history is stored in MongoDB.
    - User History
    ![Screenshot 2024-06-04 090741](https://github.com/Chamindu77/Real-Time-Chat-App/assets/117502200/87693f05-33b3-489b-b3f3-faab11427b98)

    - Message History
      ![Screenshot 2024-06-04 090754](https://github.com/Chamindu77/Real-Time-Chat-App/assets/117502200/05664fd3-684e-49ac-957f-07d37111ebcd)

    - Conversation History
      ![Screenshot 2024-06-04 090803](https://github.com/Chamindu77/Real-Time-Chat-App/assets/117502200/b0f24b9d-2cc9-459c-8da5-24f132231264)

 

### Database Attck Managment

- Cross-Site Scripting(XSS) and Cross-site Request Forgery(CSRF) are used as potential database attack vectors that could be relevent in the context of using JWT and managing user session.

## Live Demo

- Demo Link:- https://real-time-chat-app-ehdj.onrender.com/

![Screenshot 2024-06-01 141204](https://github.com/Chamindu77/Real-Time-Chat-App/assets/117502200/285c7849-6a07-4e1f-9328-9a8ce6ff66fd)

