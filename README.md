

# DevinChat App

> Real-time code collaboration and chat platform for developers

## Overview

DevinChat is a specialized chat application designed for developers to collaborate on code in real-time. It combines instant messaging with powerful development features like syntax highlighting, live code execution, and project management.

## Features

🚀 **Core Features**
- Real-time messaging using WebSocket
- Code syntax highlighting with highlight.js
- Markdown support for messages
- Project-based chat rooms
- File sharing and code snippets
- Live code execution environment
- User authentication and authorization

🔧 **Technical Features**
- WebContainer API for code execution
- Socket.io for real-time communications
- JWT-based authentication
- MongoDB for data persistence
- React with Tailwind CSS for UI
- Markdown parsing and rendering




## Features

- Real-time messaging using WebSocket
- Code syntax highlighting
- Markdown support
- Project-based chat rooms
- User authentication
- File sharing
- Code collaboration
- Responsive design

## Tech Stack

### Frontend
- React.js
- TailwindCSS
- Socket.io-client
- Markdown-to-jsx
- Axios
- React Router

### Backend
- Node.js
- Express.js
- MongoDB
- Socket.io
- JWT Authentication
- WebContainers API

## API Documentation
# Authentication
POST /api/users/register - Register new user
POST /api/users/login - Login user
GET /api/users/me - Get current user
# Projects
GET /api/projects - Get all projects
POST /api/projects - Create new project
PUT /api/projects/:id - Update project
DELETE /api/projects/:id - Delete project
# Messages
GET /api/messages/:projectId - Get project messages
POST /api/messages - Send message
DELETE /api/messages/:id - Delete message

# Code Structure
frontend/
├── src/
│   ├── components/
│   ├── context/
│   ├── hooks/
│   ├── screens/
│   └── config/
backend/
├── controllers/
├── models/
├── routes/
└── services/

# WebSocket Events
Event	Description
connection	Client connects
message	New message
code_update	Code changes
join_room	Join project

## High-Level Design

### Frontend
The frontend of the Devin Chat App is built using HTML, CSS, and JavaScript, with a focus on providing a responsive and user-friendly interface. It communicates with the backend through WebSocket and HTTP requests to enable real-time messaging and other features.

### Backend
The backend is built with Node.js and Express, providing a robust and scalable server-side architecture. It handles user authentication, message routing, chat room management, and other core functionalities. The backend also integrates with a database to store user data, messages, and other relevant information.

## Low-Level Design

### Frontend Components
- **Login Component**: Handles user authentication.
- **Chat Room Component**: Displays chat rooms and messages.
- **Message Input Component**: Allows users to type and send messages.
- **User Profile Component**: Displays and allows editing of user profile information.
- **Notification Component**: Displays message notifications and alerts.

### Backend Modules
- **Authentication Module**: Manages user login and registration.
- **Message Module**: Handles sending, receiving, and storing messages.
- **Chat Room Module**: Manages chat room creation, deletion, and user participation.
- **Notification Module**: Sends notifications for new messages and other events.
- **User Module**: Manages user profiles and presence indicators.

## Additional Features
- **Voice and Video Calls**: Users can make voice and video calls within the app.
- **End-to-End Encryption**: Ensures secure communication between users.
- **Customizable Themes**: Users can customize the app's appearance.
- **Integration with Third-Party Services**: Supports integration with services like Google Drive and Dropbox.
- **Moderation Tools**: Admins can moderate chat rooms and manage user behavior.
- **Analytics**: Provides insights into user activity and engagement.
- **API Access**: Developers can access the app's API to build custom integrations.
- **Support for Bots**: Users can add and interact with chatbots in chat rooms.
- **Multi-Device Sync**: Users can access their chats from multiple devices.
- **Offline Messaging**: Users can send messages even when offline, which will be delivered when they come online.
- **Scheduled Messages**: Users can schedule messages to be sent at a later time.
- **Custom Emojis and Stickers**: Users can create and use custom emojis and stickers.
- **Polls and Surveys**: Users can create polls and surveys in chat rooms.
- **Threaded Conversations**: Supports threaded conversations for better message organization.
- **Message Reactions**: Users can react to messages with emojis.
- **Customizable Notifications**: Users can customize notification settings for different chat rooms and messages.
- **Data Export**: Users can export their chat data for backup or analysis.
- **Two-Factor Authentication**: Adds an extra layer of security for user accounts.
- **Single Sign-On (SSO)**: Supports SSO for enterprise users.
- **Custom Domains**: Users can use custom domains for their chat rooms.
- **Webhooks**: Supports webhooks for real-time notifications and integrations.
- **Role-Based Access Control**: Admins can assign roles and permissions to users.
- **Audit Logs**: Keeps track of user activity and changes in the app.
- **Custom Commands**: Users can create and use custom commands in chat rooms.
- **Message Formatting**: Supports rich text formatting for messages.
- **Auto-Moderation**: Automatically moderates chat rooms based on predefined rules.
- **Customizable User Interface**: Users can customize the app's user interface to suit their preferences.
- **Multi-Tenancy**: Supports multiple tenants with isolated data and configurations.
- **Scalability**: Designed to handle a large number of users and messages.
- **Performance Optimization**: Optimized for fast and efficient performance.

## File Structure

### Frontend
- `index.html`: Main HTML file.
- `styles.css`: Main CSS file.
- `app.js`: Main JavaScript file.
- `components/`: Contains individual frontend components.
   - `LoginComponent.js`: Handles user authentication.
   - `ChatRoomComponent.js`: Displays chat rooms and messages.
   - `MessageInputComponent.js`: Allows users to type and send messages.
   - `UserProfileComponent.js`: Displays and allows editing of user profile information.
   - `NotificationComponent.js`: Displays message notifications and alerts.

### Backend
- `server.js`: Entry point of the application.
- `routes/`: Contains route definitions for API endpoints.
   - `authRoutes.js`: Routes for authentication.
   - `messageRoutes.js`: Routes for message handling.
   - `chatRoomRoutes.js`: Routes for chat room management.
   - `notificationRoutes.js`: Routes for notifications.
   - `userRoutes.js`: Routes for user management.
- `controllers/`: Contains logic for handling requests.
   - `authController.js`: Logic for authentication.
   - `messageController.js`: Logic for message handling.
   - `chatRoomController.js`: Logic for chat room management.
   - `notificationController.js`: Logic for notifications.
   - `userController.js`: Logic for user management.
- `models/`: Contains database models.
   - `User.js`: User model.
   - `Message.js`: Message model.
   - `ChatRoom.js`: Chat room model.
   - `Notification.js`: Notification model.
- `public/`: Contains static files for the client-side application.

## Flow Chart

graph TD;
    A[Client] -->|WebSocket| B[Server];
    B --> C[Authenticate User];
    B --> D[Route Messages];
    B --> E[Handle Chat Rooms];
    C --> F[Database];
    D --> F;
   
   
Contact -
Name - @mdaaman77

Project Link: https://github.com/mdaaman77/Devin-chatApp 



