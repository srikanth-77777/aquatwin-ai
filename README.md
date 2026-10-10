AquaTwin AI

Urban Water Network Digital Twin Dashboard

AquaTwin AI is a real-time digital twin platform designed for monitoring and simulating urban water networks. It features a Node.js backend providing both REST APIs and a WebSocket-based real-time engine to serve sensor updates, network statuses, alerts, and AI logs to a frontend dashboard.

Live Demo

A live demonstration of the AquaTwin AI server can be accessed here:

https://aquatwin-ai.onrender.com

Features
Real-time Dashboard: Live data streaming and updates via WebSockets.
Network Simulation: Automatic background generation of sensor readings and network events.
RESTful APIs: Endpoints to interact with network nodes, sensors, alerts, and predictive scenarios (/api/network, /api/sensors, /api/alerts, /api/scenarios).
Local Storage: Leverages SQLite (better-sqlite3) for lightweight, robust local data storage.
Prerequisites
Node.js
 (v14 or newer recommended)
npm (comes with Node.js)
Installation
Clone the repository or download the source code.
Navigate to the project directory (if not already there):
bash
cd "aqua ai"
Install the required dependencies:
bash
npm install
Usage
Starting the Server

For development with automatic server restarts (via nodemon):

bash
npm run dev

For standard execution:

bash
npm start
Accessing the System

Once the server is running, the following endpoints will be active:

Web Dashboard (UI): http://localhost:3000
Health Check API: http://localhost:3000/api/health
WebSocket Engine: ws://localhost:3000
Technologies Used
Backend: Node.js, Express.js
Real-time Engine: WebSockets (ws)
Database: SQLite (better-sqlite3)
