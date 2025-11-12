# 🚀 EtherLink P2P
**High-end browser-based peer-to-peer chat and video platform using HTML, CSS, and JavaScript**

---

## 📌 Project Overview

EtherLink P2P is a **fully client-side peer-to-peer chat and video communication platform**, built with **HTML, CSS, and JavaScript**. It leverages **WebRTC** and **PeerJS** for direct peer connections, enabling:

- Real-time **video/audio calls** 🎥🎤  
- **File sharing** 📁  
- Interactive **chat messaging** 💬  
- Advanced UI features like **typing indicators** ⌨️ and **emoji reactions** 😄  

All features run **without a backend server**, directly in the browser. The interface is modern, responsive, and inspired by professional chat apps like Slack and Discord.  

---

## ✨ Key Features

### Core Features

## 🎥 Real-Time Video & Audio Chat
- Full-duplex video and audio streaming using **WebRTC**  
- Local and remote video previews with dynamic resizing  
- Toggle buttons to enable/disable audio or video  

## 💬 Text Messaging
- Real-time chat with **timestamps**  
- Smooth **fade-in animations** for messages  
- Customizable chat bubbles for self and peers  

## 📁 File Sharing
- Drag-and-drop or standard file input support  
- **In-chat previews** for images and videos  
- Downloadable files for other types (PDFs, docs, etc.)  

## ⌨️ Typing Indicators
- Shows **"Peer is typing..."** dynamically  

## 😄 Emoji Reactions
- Custom emoji reactions for messages  
- Real-time updates for all peers  

## 🎨 High-End UI/UX
- Dark theme with gradients, rounded corners, and shadows  
- Smooth animations for messages, file previews, and hover effects  
- Fully **responsive layout** for desktop and mobile  

## 🔒 Security (Optional)
- AES-GCM encryption can be added for messages and file transfers  

---

## 🛠️ Technology Stack

| Layer             | Technology / Tool                         |
| ----------------- | ----------------------------------------- |
| Frontend          | HTML5, CSS3, JavaScript ES6               |
| P2P Communication | WebRTC, PeerJS (signaling server)         |
| Media Handling    | getUserMedia API, Video & Audio Tracks    |
| Styling           | Flexbox & CSS Grid, Animations, Gradients |
| File Handling     | FileReader API, Blob, URL.createObjectURL |
| Security          | Web Crypto API (AES-GCM)                  |

---

## 🏗️ Architecture

```text
+------------------+          +------------------+
|                  |          |                  |
|    Browser 1     |<-------> |    Browser 2     |
|                  |  P2P     |                  |
|  HTML/CSS/JS     | WebRTC   | HTML/CSS/JS      |
|                  |          |                  |
|  - Video Stream  |          |  - Video Stream  |
|  - Chat & Files  |          |  - Chat & Files  |
+------------------+          +------------------+

       ^                              ^
       |                              |
       | Signaling via PeerJS         |
       | (Public Server)              |
       v                              v

 +--------------------------------------------+
 |          PeerJS Signaling Server           |
 | - Handles peer discovery                   |
 | - Exchanges SDP offers & ICE candidates   |
 | - Media streams remain P2P, never on server
 +--------------------------------------------+
```
----

## 🚀 Installation & Usage

## 1️⃣ Clone the Repository
```text
git clone https://github.com/<username>/etherlink-p2p.git
cd etherlink-p2p
```

## 2️⃣ Open in Browser

 Open index.html in any modern browser
 Chrome, Firefox, Edge, Safari supported
 ```text
open index.html
```

## 3️⃣ Connect to a Peer

+ Enter your Peer ID (auto-generated if empty)

+ Enter the Peer ID of the other participant

+ Click Connect

+ Video/audio streams start automatically 🎥🎤

## 4️⃣ Using Chat & Files

+ Type a message and click Send 💬

+ Upload files via the file input or drag-and-drop 📁

+ View file previews (images/videos)

+ React with emojis 😄

+ See typing indicators ⌨️
  
---

🗂️ File Structure
```text
etherlink-p2p/
│
├── index.html       # Main HTML file
├── style.css        # Dark theme, animations, responsive layout
├── app.js           # JavaScript for WebRTC, chat, files, typing, emoji
├── README.md        # Project documentation
└── assets/          # Optional: icons, emoji, screenshots

```
----

## 🌐 Browser APIs Used

- WebRTC (RTCPeerConnection, getUserMedia) for P2P media streaming

- PeerJS for signaling and peer ID management

- FileReader API for file uploads and ArrayBuffer handling

- Blob & URL.createObjectURL for file previews/downloads

- Web Crypto API (Optional) for AES encryption

- Flexbox & CSS Grid for responsive layout

- CSS Animations for smooth interactions

## 🔮 Future Enhancements

- Multi-peer rooms for group chats and video conferences 👥

- Drag-and-drop file uploads with inline previews (Slack style) 📂

- Customizable themes (dark/light/gradient) 🎨

- Push notifications for offline users 🔔

- Full end-to-end encryption for messages and media 🔒

## ✅ Conclusion

EtherLink P2P is a professional-grade, browser-only P2P chat and video platform designed for high-end UI/UX, secure communication, and real-time interactivity. Its client-side architecture ensures privacy, low latency, and accessibility without relying on a backend server. With video/audio calls, chat, file sharing, typing indicators, and emoji reactions, EtherLink P2P is ideal for personal use and small team collaboration.
