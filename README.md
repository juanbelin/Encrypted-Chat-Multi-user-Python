<h1>Encrypted-Chat-Multi-user-Python 🔒💬</h1>


<h2>📜 Description</h2>

<p><strong>Encrypted-Chat-Multi-user-Python</strong> is a Python-based project designed to enable secure communication between multiple users in real time. The system leverages encryption techniques to ensure messages are protected from unauthorized access during transmission.</p>

<p>This project is ideal for learning about network programming, encryption, and real-time chat system development using Python's powerful libraries such as <code>socket</code> and <code>ssl</code>.</p>


---

<h2>📂 Contents</h2>

<ul>
  <li><strong>server.py</strong>: The main server script that manages client connections and relays encrypted messages.</li>
  <li><strong>client.py</strong>: The client-side script for connecting to the server, sending, and receiving messages.</li>
  <li><strong>README.md</strong>: Project documentation and instructions.</li>
  <li><strong>Example</strong>: Chat real example.</li>
</ul>

---

<h2>⚙️ How it Works</h2>

<p>This project uses a client-server architecture to facilitate encrypted communication between users:</p>
<p>Server:

A secure server with TLS/SSL is configured.
It listens for incoming connections, handles clients concurrently and relays messages to other connected users.
It provides a command (!users) to list active users in the chat.</p>
<p></p>
Client:

Each user connects to the server by entering a username.
The graphical interface (with Tkinter) allows sending messages, listing connected users and logging out.
Messages are transmitted encrypted to preserve privacy.</p>

---

<h2>🎥 Certificates generation</h2>
<p>You can create the certificates with the next comandas in Linux:</p>
<p><code>openssl genpkey -algorithm RSA -out server-key.key -aes256</code></p>
<p><code>openssl req -new -key server-key.key -out server.csr</code></p>
<p><code>openssl x509 -req -days 365 -in server.csr -signkey server-key.key -out server-cert.pem</code></p>
<p><code>openssl rsa -in server-key.key -out server-key.key </code></p>


---

<h2>🔒 Conclusion</h2>

<p>Encrypted-Chat-Multi-user-Python demonstrates the integration of cryptography and network programming in a simple yet practical project. It is a great starting point for developers looking to explore secure communication systems.</p>

