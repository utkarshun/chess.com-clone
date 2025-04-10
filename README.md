# ♟️ Chess.com Clone (Multiplayer)

This project is a real-time multiplayer Chess.com clone built with **Node.js**, **Express**, **Socket.IO**, and the **chess.js** library. It features drag-and-drop gameplay, real-time synchronization, player roles, and clean UI styling.

---

## 🌐 Live Demo (Optional)

> _Add your live link here if deployed (e.g., on Render, Vercel, etc.)_

---

## 📁 Project Structure

chess/
├── app.js                      # Main backend server (Express + Socket.IO)
├── package.json
├── package-lock.json
├── style.css                   # Global stylesheet (currently empty)
├── views/
│   └── index.ejs               # Main HTML template served by Express
├── public/                     # Static files served to client
│   ├── css/                    # (Add your custom stylesheets here if needed)
│   └── js/
│       └── chessgame.js        # Frontend logic (drag-and-drop, socket events)
├── files/                      # Backup or zipped files (ignored in prod)
├── backendSetup.yaml           # Optional: Backend deployment config
└── frontendSetup.yaml          # Optional: Frontend deployment config


## 🚀 Features

- ♟️ Drag-and-drop chess pieces
- 🔄 Real-time move sync using WebSockets
- 🎭 Role assignment: White, Black, Spectator
- 🧠 Chess logic handled by chess.js (move validation, FEN state)
- 🖥️ Chessboard rendering using HTML/CSS grid

---

## 🧰 Technologies Used

### Frontend
- HTML5, CSS3
- Vanilla JavaScript
- [Socket.IO Client](https://socket.io/)
- Unicode chess pieces

### Backend
- Node.js
- Express.js
- [Socket.IO](https://socket.io/)
- [chess.js](https://github.com/jhlywa/chess.js)

---

## 📦 Installation

```bash
git clone https://github.com/your-username/chess-com-clone.git
cd chess-com-clone
npm install
node app.js
```

Then open your browser and go to:  
[http://localhost:3000](http://localhost:3000)

📸 Screenshots


✍️ How It Works
🧠 Backend (app.js)
Sets up a Socket.IO server.

Maintains the current game state using chess.js.

Assigns roles to players (white, black, spectator).

Broadcasts moves to all clients in real time.

Sends updated board state using FEN strings.

🎮 Frontend (chessgame.js)
Renders the chessboard using DOM manipulation.

Uses drag-and-drop to allow piece movement.

Converts source and target squares to algebraic notation.

Emits valid moves via Socket.IO.

Updates board based on server-sent FEN state.

🛠️ TODO / Future Improvements
✅ Pawn promotion support

❌ Move history log

❌ Game timer

❌ Checkmate / draw notifications

❌ Restart game button

❌ Deploy to live hosting (Render, Vercel, etc.)

🙌 Acknowledgements
chess.js for chess logic

Socket.IO for real-time WebSocket communication

📃 License
This project is licensed under the MIT License.

👤 Author
Utkarsh Kher
GitHub: @your-username
LinkedIn: linkedin.com/in/utkarsh-kher-654a1a282
