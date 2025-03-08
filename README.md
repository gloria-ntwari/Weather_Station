MQTT Weather Station Dashboard 🌡️💧
Real-time weather monitoring with MQTT, SQLite storage, and a sleek dashboard showing live data and 5-minute averages.

Features
🌡️ Real-time temperature & humidity

📊 Interactive charts with historical data

💾 SQLite database storage

📱 Responsive UI

Setup Instructions
Prerequisites: Node.js (v14+), npm, Git

Clone repo: git clone <your-repo-url>
Install dependencies: npm install
Create public/ folder, add index.html
Start server: node server.js
Access app: http://localhost:3000
Project Structure
text

Collapse

Wrap

Copy
weather-station/  
├── public/  
│   └── index.html  # Frontend UI  
├── server.js       # Backend logic  
├── package.json    # Dependencies  
├── weather_data.db # SQLite DB  
└── README.md       # Instructions  
How It Works
Frontend connects to MQTT broker for real-time data
Backend stores data in SQLite, calculates 5-min averages
Charts show up to 1 hour of historical data
API Endpoints
POST /api/weather/data - Store readings
GET /api/weather/history - Fetch historical data
Run in Terminal 🖥️
Navigate to directory
Run node server.js or visit http://localhost:3000