
<body>

  <h1>MERN Chat Application</h1>
  <p>
    A full-stack real-time chat application built using the <strong>MERN</strong> stack (MongoDB, Express, React, Node.js).
    This application allows users to create an account, join chat rooms, and send real-time messages using web sockets.
  </p>

  <h2>Features</h2>
  <ul>
    <li><strong>User Authentication</strong>: Register and log in to your account.</li>
    <li><strong>Real-time Messaging</strong>: Chat with other users in real-time using <code>Socket.io</code>.</li>
    <li><strong>Multiple Chat Rooms</strong>: Join different rooms and have separate conversations.</li>
    <li><strong>Responsive Design</strong>: Mobile and desktop friendly.</li>
    <li><strong>MongoDB Database</strong>: User accounts and messages are stored in a MongoDB database.</li>
    <li><strong>Notifications</strong>: Receive real-time notifications for new messages.</li>
    <li><strong>Secure</strong>: Passwords are hashed and sensitive data is protected.</li>
  </ul>

  <h2>Tech Stack</h2>
  <ul>
    <li><strong>Frontend</strong>: React, CSS</li>
    <li><strong>Backend</strong>: Node.js, Express.js</li>
    <li><strong>Database</strong>: MongoDB, Mongoose</li>
    <li><strong>Real-time Communication</strong>: Socket.io</li>
    <li><strong>Authentication</strong>: JWT (JSON Web Tokens), bcrypt</li>
    <li><strong>Deployment</strong>: Render/Heroku, MongoDB Atlas</li>
  </ul>

  <h2>Screenshots</h2>
  <p><em>Include screenshots or GIFs of your application in action.</em></p>

  <h2>Getting Started</h2>
  <h3>Prerequisites</h3>
  <p>To run this project locally, ensure you have the following installed:</p>
  <ul>
    <li><strong>Node.js</strong> (v12+)</li>
    <li><strong>MongoDB</strong> (Local or MongoDB Atlas)</li>
  </ul>

  <h3>Installation</h3>
  <ol>
    <li>Clone the repository:
      <pre><code>git clone https://github.com/gulshan0300/Chat_Application</code></pre>
    </li>
    <li>Navigate to the project directory:
      <pre><code>cd Chat_Application</code></pre>
    </li>
    <li>Install dependencies for both <strong>backend</strong> and <strong>frontend</strong>:
      <pre><code>
# Install backend dependencies
cd backend
npm install

# Install frontend dependencies
cd ../frontend
npm install
      </code></pre>
    </li>
    <li>Create a <code>.env</code> file in the root directory of your <strong>backend</strong> with the following values:
      <pre><code>
MONGO_URI=your-mongo-db-uri
JWT_SECRET=your-jwt-secret
      </code></pre>
    </li>
  </ol>

  <h3>Running the Application</h3>
  <ol>
    <li>Start the <strong>backend server</strong>:
      <pre><code>cd backend
node index.js</code></pre>
    </li>
    <li>Start the <strong>frontend development server</strong>:
      <pre><code>cd frontend
npm start</code></pre>
    </li>
    <li>Open the app in your browser at <code>http://localhost:3000</code>.</li>
  </ol>

  <h2>Usage</h2>
  <ul>
    <li><strong>Register</strong>: Create a new account.</li>
    <li><strong>Login</strong>: Log in with your account credentials.</li>
    <li><strong>Join Chat Rooms</strong>: Enter a chat room to start messaging with other users.</li>
    <li><strong>Send Real-time Messages</strong>: Communicate with other users instantly in real-time.</li>
  </ul>

  <h2>Folder Structure</h2>
  <div class="folder-structure">
<pre>
mern-chat-app/
│
├── backend/
│   ├── controllers/     # Route handlers
│   ├── models/          # Mongoose models (User, Message)
│   ├── routes/          # API endpoints
│   ├── config/          # Configuration files (e.g., MongoDB connection)
│   ├── middleware/      # Middleware for authentication
│   ├── server.js        # Entry point for the backend server
│
├── frontend/
│   ├── src/
│   │   ├── components/  # React components (Chat, Login, Register)
│   │   ├── pages/       # Pages (Home, ChatRoom, etc.)
│   │   ├── App.js       # Main React component
│   │   ├── index.js     # React entry point
│
└── README.md            # Project documentation
</pre>
  </div>

  <h2>Dependencies</h2>
  <h3>Backend</h3>
  <ul>
    <li><code>express</code>: Fast, unopinionated web framework for Node.js</li>
    <li><code>mongoose</code>: Elegant MongoDB object modeling for Node.js</li>
    <li><code>bcrypt</code>: Password hashing function</li>
    <li><code>jsonwebtoken</code>: JWT for authentication</li>
    <li><code>socket.io</code>: Real-time web socket communication</li>
  </ul>
  
  <h3>Frontend</h3>
  <ul>
    <li><code>react</code>: A JavaScript library for building user interfaces</li>
    <li><code>axios</code>: Promise-based HTTP client for the browser</li>
    <li><code>socket.io-client</code>: Client-side library for WebSocket communication</li>
  </ul>

  <h2>API Endpoints</h2>
  <h3>Auth Routes</h3>
  <ul>
    <li><code>POST /api/auth/register</code> - Register a new user</li>
    <li><code>POST /api/auth/login</code> - Authenticate a user</li>
  </ul>

  <h3>Chat Routes</h3>
  <ul>
    <li><code>GET /api/chat/rooms</code> - Get list of available chat rooms</li>
    <li><code>POST /api/chat/message</code> - Send a message to a room</li>
    <li><code>GET /api/chat/messages/:roomId</code> - Get messages for a specific chat room</li>
  </ul>

  <h2>Deployment</h2>
  <p>
    This application can be deployed on platforms like <a href="https://www.heroku.com/">Heroku</a> or <a href="https://render.com/">Render</a>.
  </p>
  <ol>
    <li>Set up environment variables for <code>MONGO_URI</code> and <code>JWT_SECRET</code> on the hosting platform.</li>
    <li>Deploy the backend and frontend separately or as one full-stack project.</li>
  </ol>

  <h2>Contributing</h2>
  <p>
    If you'd like to contribute to this project, feel free to open a pull request or submit an issue.
  </p>

  <h2
