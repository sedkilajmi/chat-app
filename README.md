Real-Time Chat Application
A real-time chat application built with Node.js, Express, and Socket.IO that allows users to join chat rooms, send messages, and share their live location instantly.
🚀 Features
🔌 Real-time messaging using WebSockets (Socket.IO)
👥 Multiple chat rooms support
📍 Share live location with other users
🚫 Profanity filter (bad-words package)
📢 Join / Leave room notifications
🧑 Active users list per room
🎨 Simple and clean UI
🛠️ Tech Stack
Backend:
Node.js
Express.js
Socket.IO
bad-words (profanity filter)
Frontend:
HTML5
CSS3
JavaScript
Mustache.js (templating)
Moment.js (date formatting)
Qs (query string parsing)

📂 Project Structure
project-root
│
├── src
│   ├── index.js
│   ├── utils
│   │   ├── messages.js
│   │   └── users.js
│
├── public
│   ├── index.html
│   ├── chat.html
│   ├── css
│   ├── js
│   └── img
│
├── package.json
└── README.md

⚙️ Installation & Setup
1️⃣ Clone repository
git clone https://github.com/YOUR_USERNAME/YOUR_REPO.git
2️⃣ Navigate to project folder
cd YOUR_REPO
3️⃣ Install dependencies
npm install
4️⃣ Run the server
npm run start

🌐 Usage

Open browser
Go to:
http://localhost:3000
Enter:
Username
Room name
Start chatting 🎉
🔄 Socket Events
Client → Server

join → Join chat room
sendMessage → Send message
sendLocation → Share location
Server → Client
message → Receive message
locationMessage → Receive location
roomData → Users list update
🧠 How It Works
Users connect via Socket.IO
Server manages users in memory
Messages are broadcast only to room members
Location is shared using Google Maps link
Profanity is filtered before sending messages
