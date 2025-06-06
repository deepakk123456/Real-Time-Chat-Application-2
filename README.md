A real-time chat application built using Node.js, Express, MongoDB, Socket.IO, and React.js. This app supports user authentication, 1-on-1 chat, group chats, real-time messaging, and notifications, providing a seamless and interactive messaging experience.

🚀 Features
🔐 User Authentication (Register/Login with JWT)

👤 1-on-1 Private Chat

👥 Group Chat Functionality

📡 Real-time Messaging with Socket.IO

🛎️ Message Notifications

🖼️ Support for Emojis and Image Uploads (optional)

🌐 RESTful API with Express.js

🎨 Modern, responsive UI built with React.js

🛠️ Tech Stack
🔧 Backend
Node.js

Express.js

MongoDB + Mongoose

Socket.IO

JSON Web Tokens (JWT)

bcrypt.js

🎨 Frontend
React.js

Axios

React Router

Socket.IO Client

📁 Project Structure
pgsql
Copy
Edit
📦 real-time-chat-app
├── server/               # Backend code
│   ├── config/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   └── socket/
├── client/               # Frontend code
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── context/
│   │   └── App.jsx
├── .env
├── package.json
└── README.md
⚙️ Installation
1. Clone the repository
bash
Copy
Edit
git clone https://github.com/your-username/real-time-chat-app.git
cd real-time-chat-app
2. Setup Backend
bash
Copy
Edit
cd server
npm install
Create a .env file in the server/ directory:

env
Copy
Edit
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
PORT=5000
Start the server:

bash
Copy
Edit
npm run dev
3. Setup Frontend
Open a new terminal:

bash
Copy
Edit
cd client
npm install
npm run dev
Frontend runs at: http://localhost:5173

🔄 API Endpoints
Auth Routes
POST /api/auth/register

POST /api/auth/login

User Routes
GET /api/users

GET /api/users/:id

Chat Routes
POST /api/chats

GET /api/chats

POST /api/chats/group

PUT /api/chats/group/rename

PUT /api/chats/group/add

PUT /api/chats/group/remove

Message Routes
POST /api/messages/:chatId

GET /api/messages/:chatId

🔒 Authentication
Passwords are hashed using bcrypt.js

JWT tokens are used for secure authentication and stored in localStorage or HTTP-only cookies (based on your setup)

⚡ Real-Time Messaging
Socket.IO is used for bi-directional communication between the client and server.

Users get instant message delivery, typing indicators, and message notifications.

📸 Screenshots
(Include screenshots here of login page, chat window, group chat interface, etc.)

🧪 Future Enhancements
✅ Online/offline user indicator

✅ Audio/Video calling with WebRTC

✅ Read receipts

✅ File sharing (PDFs, images)

✅ Dark mode support

🤝 Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

📄 License
This project is licensed under the MIT License.

📬 Contact
Deepak Kainthola
📧 Email: [deepakkainthola31@gmail.com]
