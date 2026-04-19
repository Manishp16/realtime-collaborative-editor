# 🚀 Realtime Editor

A real-time collaborative code editor that allows multiple users to edit code simultaneously.

## ✨ Features

- 👥 Real-time collaboration with multiple users
- 📝 Monaco Editor (VS Code's editor)
- 🔄 Automatic synchronization with CRDT
- 💬 See who's currently editing
- ⚡ Hot reload in development
- 🐳 Docker ready

## 🚀 Quick Start

### Prerequisites
- Node.js 20+
- npm 9+

### Installation

```bash
# Backend
cd Backend
npm install
npm run dev

# Frontend (in another terminal)
cd Frontend
npm install
npm run dev
```

Open `http://localhost:5173` and start editing!

### Test Collaboration

1. Open first tab: `http://localhost:5173?username=Alice`
2. Open second tab: `http://localhost:5173?username=Bob`
3. Type in one → see changes in the other ✨

## 📁 Project Structure

```
├── Backend/
│   ├── server.js          # Express + Socket.io server
│   └── package.json       # Dependencies
├── Frontend/
│   ├── src/
│   │   └── app/
│   │       └── App.jsx    # Main editor component
│   └── package.json       # Dependencies
├── dockerfile             # Docker build
└── README.md             # This file
```

## 🛠️ Technologies

- **Frontend**: React, Vite, Monaco Editor, Tailwind CSS
- **Backend**: Express, Socket.io
- **Sync**: Yjs (CRDT), y-socket.io

## 🐳 Docker

```bash
docker build -t realtime-editor .
docker run -p 3000:3000 realtime-editor
```

Access at `http://localhost:3000`

## � Commands

**Backend:**
- `npm run dev` - Start with auto-reload
- `npm start` - Start production server

**Frontend:**
- `npm run dev` - Start dev server
- `npm run build` - Build for production
- `npm run lint` - Run ESLint

## 👨‍💻 Author

Add your name here!

---

**Happy coding! 🎉**
