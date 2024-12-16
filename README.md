# Chat Application 📡💬

A lightweight and user-friendly chat application built with Python. This project includes a **server** to manage connections and a **client** with a graphical user interface for seamless communication.

---

## Features 🌟

- **Real-time Messaging:** Exchange messages instantly between connected users.
- **User-Friendly Interface:** Simple GUI built with `Tkinter` for intuitive usage.
- **Custom Alignment:** Sent and received messages are aligned to the right and left, respectively.
- **Scalable Server:** Handles multiple connections efficiently using non-blocking I/O.
- **Customizable IP & Port:** Easily configure the server and client to run on different networks.

---

## Technology Stack 🛠️

- **Frontend (Client):**
  - `Tkinter` for GUI
  - `socket` for networking
  - `threading` for concurrent operations
- **Backend (Server):**
  - `socket` for networking
  - `select` for handling multiple connections
- **Protocol:** TCP with custom message headers for structured communication.

---

## Setup and Usage 🚀

### 1. Clone the Repository
```bash
git clone <repository-link>
cd <repository-folder>
```

### 2. Run the Server
1. Navigate to the project folder.
2. Start the server:
   ```bash
   python Server.py
   ```
3. The server will listen for incoming connections on `0.0.0.0:3000` by default.

### 3. Run the Client
1. Navigate to the project folder.
2. Start the client:
   ```bash
   python Client.py
   ```
3. Enter a username when prompted and start chatting!

---

## Screenshots 📸

### Chat Interface (Client)
![image](https://github.com/user-attachments/assets/7a4cc23f-7c17-4fd1-92b3-42becd37ec4f)


---

## How It Works ⚙️

1. **Server**:
   - Listens for incoming client connections.
   - Maintains a list of connected clients.
   - Broadcasts messages from one client to all others.

2. **Client**:
   - Connects to the server using IP and port.
   - Provides a GUI for users to send and view messages.
   - Uses threading to handle incoming messages without freezing the interface.

---

## Configuration 🔧

### Server
- **IP:** Default is `0.0.0.0`.
- **Port:** Default is `3000`.

To change the settings, update these lines in `Server.py`:
```python
IP = "0.0.0.0"
PORT = 3000
```

### Client
- **IP:** Update to the server's IP address.
- **Port:** Match the server's port.

Modify these lines in `Client.py`:
```python
IP = "10.113.18.221"
PORT = 3000
```

---

## Contribution 🤝

We welcome contributions to improve this project! Feel free to fork the repository and submit pull requests.

---

## License 📜

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).

---

## Acknowledgments ❤️

Special thanks to the open-source community for providing inspiration and resources.
