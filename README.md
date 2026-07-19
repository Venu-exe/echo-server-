# Python TCP Echo Server

A simple, safe, and robust TCP Echo Server written in native Python. This project is a great foundational example for learning network programming and socket handling.

## Features
- Listens on `localhost:8080` (TCP)
- Gracefully handles client connections and disconnections
- Immediately releases the bound port on exit using `SO_REUSEADDR`
- Safely echoes received data back to the client without executing system commands

## Usage

### 1. Start the Server
Run the script in your terminal to start the server. It will begin listening on port 8080.
```bash
python simple.py
```

### 2. Connect with a Client
Open a **new** terminal window and connect to the server using `netcat` (or `telnet`).
```bash
nc 127.0.0.1 8080
```

Once connected, anything you type into the netcat terminal will be sent to the server and safely echoed right back to you.

### 3. Stop the Server
To stop the server, press `Ctrl+C` in the terminal where it is running.
