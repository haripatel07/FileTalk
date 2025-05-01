# FileTalk

**FileTalk** is a multi-client chat and file-sharing application built in Java, designed for use within a Local Area Network (LAN). It allows multiple users to chat with each other and exchange files in real-time, all while handling client-server communication efficiently.

## Features

- **Multi-client support**: Multiple clients can connect to the server and communicate with each other.
- **Text messaging**: Real-time chat functionality between clients.
- **File sharing**: Clients can send and receive files with each other.
- **Graceful disconnection**: Clients can exit the chat and close the connection with a simple command.

## Technologies Used

- **Java**: Core programming language for building both the client and server.
- **Socket Programming**: For establishing communication between server and multiple clients.
- **Multi-threading**: Handling multiple client connections concurrently.
- **File I/O**: For file transfers between the server and clients.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/haripatel07/FileTalk.git
   ```

2. Navigate to the project directory:
   ```bash
   cd FileTalk
   ```

3. Compile the Java files:
   ```bash
   javac Server.java Client.java
   ```

## Usage

### 1. Run the Server
Start the server to listen for incoming client connections:
```bash
java Server
```

### 2. Run the Client
Start a client on any machine connected to the same LAN:
```bash
java Client
```

### 3. Interact with the Chat
- Type messages to communicate with the server or other clients.
- To send a file, type `sendfile <path_to_file>` in the client console.
- The server will notify when a file is received or ready to be downloaded.

### 4. Exit the Chat
To disconnect from the server, simply type `exit` in the client console.

## Example Commands

- **Send message**: `Hello, Server!`
- **Send file**: `sendfile /path/to/file.txt`
- **Exit**: `exit`

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
