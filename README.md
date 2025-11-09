# Network-File-Sharing-Server-Client-using-C-Socket-Programming

# 🌐 Network File Sharing System (C++)

A **Client–Server File Sharing Application** built in **C++** using **TCP sockets**.  
It allows **secure file uploads and downloads** with **basic authentication** and **XOR-based encryption**.

---

## 🚀 Features

✅ Server–Client socket communication  
✅ File listing, upload, and download  
✅ Basic user authentication (user/password)  
✅ Simple XOR encryption for file data  
✅ Modular and extendable design  

---

## 🧩 Tech Stack

| Component | Technology |
|------------|-------------|
| Language | C++ (C++17) |
| Communication | TCP Sockets (POSIX) |
| OS Compatibility | Linux / macOS / WSL |
| Security | Simple XOR Encryption |

---

## 🧱 Folder Structure

Network-File-Sharing-Cpp/
│
├── server.cpp # Server-side source code
├── client.cpp # Client-side source code
├── README.md # Project documentation
├── .gitignore # Ignored files list
└── demo/ # Screenshots or demo files (optional)

yaml
Copy code

---

## ⚙️ How to Build & Run

### 1️⃣ Compile
```bash
g++ -std=c++17 -O2 server.cpp -o server
g++ -std=c++17 -O2 client.cpp -o client
2️⃣ Start the Server
bash
Copy code
./server 8080
3️⃣ Start the Client
bash
Copy code
./client 127.0.0.1 8080
🔐 Login Credentials
pgsql
Copy code
Username: user
Password: password
💬 Available Commands
Command	Description
LIST	Show files available on server
GET <filename>	Download a file from server
PUT <filename>	Upload a file to server
QUIT	Disconnect client

🧠 Example Output
🖥️ Server
arduino
Copy code
Server listening on port 8080 …
Client connected.
Auth OK.
Connection closed.
💻 Client
vbnet
Copy code
Authenticated.

Commands:
1) LIST
2) GET <filename>
3) PUT <filename>
4) QUIT

Choose: 1
Available files:
1. report.txt
2. image.png
🔒 Encryption
A simple XOR cipher is used to encrypt and decrypt file bytes during transfer:

cpp
Copy code
for (size_t i = 0; i < size; ++i)
    data[i] ^= 'K';  // XOR encryption key
You can replace this with AES/TLS for stronger security.

🧾 Future Improvements
🔁 Add multithreading for multiple clients

🔒 Implement AES or TLS-based encryption

🗃️ Add authentication database for multiple users

🌐 Add web dashboard using Flask/React

📸 Demo Screenshots
(Place screenshots inside /demo folder and reference them below)



🧑‍💻 Author
Harsh Kumar Singh
🎓 B.Tech Cybersecurity, ITER SOA University
📧 [your-email@example.com]
🔗 LinkedIn
🔗 GitHub

🏁 License
This project is open-source under the MIT License.

yaml
Copy code

---

## 🧭 **6️⃣ Uploading to GitHub**

### Option 1 – Using Terminal

```bash
git init
git add .
git commit -m "Initial commit: Network File Sharing C++"
git branch -M main
git remote add origin https://github.com/<your-username>/Network-File-Sharing-Cpp.git
git push -u origin main
