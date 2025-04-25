# 💬 MERN Chat App

A real-time chat application built with the **MERN stack** (MongoDB, Express.js, React, Node.js) and **Socket.io**, featuring theme support with **Tailwind CSS** and **DaisyUI**.

---

## 🚀 Features

- 💬 Real-time messaging with Socket.io  
- 👥 Join and chat in public rooms  
- 🧑‍🤝‍🧑 User authentication (optional - add JWT/local auth)  
- 🌗 Theme support (light/dark/custom themes using DaisyUI)  
- 💻 Responsive UI with Tailwind CSS

---

## 🧰 Tech Stack

- **Frontend**: React, Tailwind CSS, DaisyUI, Socket.io-client  
- **Backend**: Node.js, Express, Socket.io  
- **Database**: MongoDB (Mongoose)

---

## 📦 Installation

### 1. Clone the repository

```bash
git clone https://github.com/your-username/mern-chat-app.git
cd mern-chat-app
```

### 2. Setup server

```bash
cd server
npm install
```

- Create a `.env` file in `/server` and add:
```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
```

- Start the server:
```bash
npm run dev
```

### 3. Setup client

```bash
cd ../client
npm install
```

- Start the client:
```bash
npm start
```

The app will run at: [http://localhost:3000](http://localhost:3000)

---

## 🛠️ Folder Structure

```
mern-chat-app/
├── client/              # React frontend
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── App.jsx
│   │   └── index.css    # Tailwind and DaisyUI setup
├── server/              # Express backend
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── socket.js        # Socket.io logic
│   └── server.js
```

---

## 🎨 Tailwind & DaisyUI Setup (Client Side)

**tailwind.config.js**
```js
module.exports = {
  content: ['./src/**/*.{js,jsx,ts,tsx}'],
  theme: {
    extend: {},
  },
  plugins: [require('daisyui')],
  daisyui: {
    themes: ['light', 'dark', 'cupcake', 'forest'], // you can customize themes here
  },
}
```

**index.css**
```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

---

## 🧪 Example Features

- Join Room UI with dropdown themes
- Dynamic chat updates via Socket.io
- Styled input and message bubbles via DaisyUI components
- Theme switcher using DaisyUI dropdown

---

## 📌 To Do (Optional Enhancements)

- ✅ Add private chat / DMs  
- ✅ Add user authentication (JWT or OAuth)  
- ✅ Add typing indicators  
- ✅ Add emoji support  
- ✅ Persist messages in DB

---

## 📝 License

This project is licensed under the MIT License.

---

## 💡 Inspiration

Inspired by real-time chat apps like Slack and Discord, built for learning WebSockets and MERN integration.

---
```
