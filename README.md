# 🚀 SigmaGPT

<div align="center">

![Project Status](https://img.shields.io/badge/status-active-success?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-blue?style=flat-square)
![Node.js](https://img.shields.io/badge/Node.js-18%2B-green?style=flat-square&logo=node.js)
![React](https://img.shields.io/badge/React-18%2B-blue?style=flat-square&logo=react)
![Vite](https://img.shields.io/badge/Vite-5%2B-purple?style=flat-square&logo=vite)

A powerful AI-driven chat application that leverages OpenAI's GPT models to provide intelligent conversational responses in real-time.

[Features](#-features) • [Installation](#-installation) • [Usage](#-usage) • [Tech Stack](#-tech-stack) • [Project Structure](#-project-structure)

</div>

---

## 📋 Table of Contents

- [✨ Features](#-features)
- [🛠️ Tech Stack](#-tech-stack)
- [📁 Project Structure](#-project-structure)
- [⚙️ Installation](#-installation)
- [🚀 Usage](#-usage)
- [📝 API Endpoints](#-api-endpoints)
- [🎨 Screenshots](#-screenshots)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)

---

## ✨ Features

<table>
<tr>
<td width="50%">

### 💬 Core Features
- **Real-time Chat**: Instant messaging with AI
- **Thread Management**: Organize conversations
- **Message History**: Persistent chat storage
- **Clean UI**: Modern, responsive interface

</td>
<td width="50%">

### 🔧 Technical Features
- **OpenAI Integration**: Powered by GPT models
- **Express Server**: Robust backend architecture
- **React Frontend**: Dynamic user interface
- **Vite Bundler**: Lightning-fast development

</td>
</tr>
</table>

---

## 🛠️ Tech Stack

<div align="center">

| Category | Technologies |
|----------|---------------|
| **Frontend** | React 18, Vite, CSS3 |
| **Backend** | Node.js, Express.js |
| **AI** | OpenAI API |
| **Database** | MongoDB (Thread storage) |
| **Tools** | ESLint, Git |

</div>

---

## 📁 Project Structure

```
SigmaGPT/
├── 📂 Backend/
│   ├── server.js                 # Main server entry point
│   ├── package.json              # Backend dependencies
│   ├── 📁 models/
│   │   └── Thread.js             # Thread data model
│   ├── 📁 routes/
│   │   └── chat.js               # Chat API routes
│   └── 📁 utils/
│       └── openai.js             # OpenAI API integration
│
├── 📂 Frontend/
│   ├── index.html                # Entry HTML file
│   ├── vite.config.js            # Vite configuration
│   ├── eslint.config.js          # ESLint rules
│   ├── package.json              # Frontend dependencies
│   ├── 📁 src/
│   │   ├── main.jsx              # React entry point
│   │   ├── App.jsx               # Main App component
│   │   ├── MyContext.jsx         # Context API setup
│   │   ├── Chat.jsx              # Chat component
│   │   ├── ChatWindow.jsx        # Chat window display
│   │   ├── Sidebar.jsx           # Sidebar navigation
│   │   ├── 📁 assets/            # Static assets
│   │   └── 📁 styles/
│   │       ├── App.css
│   │       ├── Chat.css
│   │       ├── ChatWindow.css
│   │       ├── Sidebar.css
│   │       └── index.css
│   └── 📁 public/                # Public static files
│
└── 📄 README.md                  # This file
```

---

## ⚙️ Installation

### Prerequisites
- **Node.js** (v18 or higher)
- **npm** or **yarn** package manager
- **OpenAI API Key** ([Get one here](https://platform.openai.com/api-keys))

### Backend Setup

```bash
# Navigate to backend directory
cd Backend

# Install dependencies
npm install

# Create .env file with your OpenAI API key
echo "OPENAI_API_KEY=your_api_key_here" > .env

# Start the server
npm start
```

### Frontend Setup

```bash
# Navigate to frontend directory
cd Frontend

# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build
```

---

## 🚀 Usage

### Starting the Application

**Terminal 1 - Start Backend:**
```bash
cd Backend
npm start
# Server runs on http://localhost:5000 (or configured port)
```

**Terminal 2 - Start Frontend:**
```bash
cd Frontend
npm run dev
# App opens at http://localhost:5173
```

### Using the Chat Interface

1. **Open the application** in your browser
2. **Type your message** in the chat input
3. **Press Enter** or click Send
4. **Wait for AI response** - the model processes your message
5. **View conversation history** in the sidebar

---

## 📝 API Endpoints

### Chat Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| `POST` | `/api/chat/send` | Send a message and get AI response |
| `GET` | `/api/threads` | Retrieve all conversation threads |
| `GET` | `/api/threads/:id` | Get specific thread messages |
| `DELETE` | `/api/threads/:id` | Delete a conversation thread |

### Request/Response Format

**Send Message Request:**
```json
{
  "message": "Hello, how are you?",
  "threadId": "optional_thread_id"
}
```

**Response:**
```json
{
  "success": true,
  "data": {
    "message": "I'm doing great, thank you for asking!",
    "threadId": "thread_123",
    "timestamp": "2024-03-22T10:30:00Z"
  }
}
```

---

## 🎨 Screenshots

| Feature | Preview |
|---------|---------|
| **Chat Interface** | Interactive messaging with real-time responses |
| **Message History** | Easy navigation through past conversations |
| **Responsive Design** | Works seamlessly on desktop and mobile |

---

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

### Steps to Contribute

1. **Fork** the repository
   ```bash
   git clone https://github.com/yourusername/SigmaGPT.git
   ```

2. **Create a feature branch**
   ```bash
   git checkout -b feature/amazing-feature
   ```

3. **Make your changes** and commit
   ```bash
   git commit -m "Add amazing feature"
   ```

4. **Push to your fork**
   ```bash
   git push origin feature/amazing-feature
   ```

5. **Open a Pull Request**

### Contribution Guidelines
- Follow the existing code style
- Add tests for new features
- Update documentation as needed
- Keep commits atomic and descriptive

---

## 📄 License

This project is licensed under the **MIT License** - see the LICENSE file for details.

---

## 🙋 Support

If you have questions or issues:
- 📧 Email: [Your Email]
- 💬 GitHub Issues: [Create an issue](https://github.com/Shubhankarmaity/SigmaGPT/issues)
- 🐛 Bug Report: [Report a bug](https://github.com/Shubhankarmaity/SigmaGPT/issues)

---

<div align="center">

**Made with ❤️ by the SigmaGPT Team**

[⭐ Star this repo](https://github.com/Shubhankarmaity/SigmaGPT) if you find it helpful!

</div>