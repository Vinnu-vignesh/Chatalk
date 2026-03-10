# Chatalk
A full-stack real-time chat application built using React &amp; Firebase, enabling users to communicate instantly with text messages and images. The application features secure authentication, live message synchronization, online status, and media sharing, providing a smooth and interactive messaging experience similar to modern chat platforms.

💬 Real-Time Chat Application

A modern Real-Time Chat Application built with React and Firebase that allows users to communicate instantly through text messages and images. The application supports live messaging, profile management, online status indicators, and media sharing, providing a smooth messaging experience similar to popular chat platforms.

The system uses Firebase Firestore for real-time database synchronization, Firebase Authentication for secure login, and Firebase Storage for media uploads.

🚀 Features
  🔐 User Authentication
  Secure user registration and login using Firebase Authentication

👤 Profile Management

  Upload and update profile picture
  Edit name and bio

💬 Real-Time Messaging
  Send and receive messages instantly
  Messages update in real time using Firestore listeners

🖼 Image Sharing
  Send images within conversations
  Images stored using Firebase Storage

🟢 Online Status
  Displays user online/offline status using lastSeen timestamp
  📁 Media Gallery

Automatically displays images shared in the conversation
  📱 Modern Chat Interface
  Sender and receiver chat bubbles
  Message timestamps
  Sidebar with user profile and shared media

🛠 Tech Stack
  Frontend
    React.js
    React Context API
    React Router
    CSS

  Backend / Cloud Services
    Firebase Authentication
    Firebase Firestore
    Firebase Storage

⚙️ Installation & Setup
1️⃣ Clone the Repository
git clone https://github.com/yourusername/realtime-chat-app.git
2️⃣ Navigate to Project Folder
cd realtime-chat-app
3️⃣ Install Dependencies
npm install
4️⃣ Configure Firebase

Create a Firebase project and replace your configuration in:

src/config/firebase.js

Example configuration:

const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "YOUR_PROJECT_ID.firebaseapp.com",
  projectId: "YOUR_PROJECT_ID",
  storageBucket: "YOUR_PROJECT_ID.appspot.com",
  messagingSenderId: "XXXX",
  appId: "XXXX"
};
5️⃣ Start the Application
npm run dev

or
npm start

🗂 Project Structure
src
│
├── assets
│
├── components
│   ├── ChatBox
│   ├── LeftSidebar
│   ├── RightSidebar
│
├── pages
│   ├── Login
│   ├── Chat
│   ├── ProfileUpdate
│
├── context
│   └── AppContext.jsx
│
├── config
│   └── firebase.js
│
└── lib
    └── upload.js
⚡ How Real-Time Messaging Works

User sends a message.
Message is stored in Firestore messages collection.
A real-time listener (onSnapshot) detects changes.
UI updates instantly without refreshing.

🎯 Future Improvements
      Message read receipts
      Typing indicator
      Group chat support
      Push notifications
      Emoji support
      Message deletion
      Voice messages

📚 What I Learned
    Through this project I gained practical experience with:
    Real-time database systems
    Firebase cloud services
    State management in React
    Building scalable chat systems
    Handling file uploads and media storage

👨‍💻 Author
Vignesh Vinnu

GitHub:
https://github.com/Vinnu-vignesh
