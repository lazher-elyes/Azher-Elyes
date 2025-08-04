# ⚡ Smart Energy Monitoring System

An end-to-end IoT-based energy monitoring and billing solution that tracks real-time electricity usage using embedded devices and provides live analytics and user dashboards via a web interface.

---

## 📌 Project Overview

This project demonstrates a scalable system for **smart energy monitoring**, combining microcontroller-based edge devices (Arduino & NodeMCU) with a full-stack web application for data visualization, billing, and device/user management.

---

## 🔧 Features

- 🔋 Real-time power consumption tracking (via sensors)
- 📲 Embedded NodeMCU-based edge device with a minimal local UI
- 📡 MQTT/HTTP communication between devices and server
- 👥 User authentication and session management
- 💳 Billing generation & payment tracking
- 📈 AngularJS web dashboard for visual analytics
- 🧠 Flask-based RESTful API for backend logic

---

## 🧰 Tech Stack

### 🔌 Hardware
- Arduino UNO
- NodeMCU ESP8266
- Current/Voltage Sensors (e.g., ACS712)

### 🖥️ Software
- Frontend: HTML, CSS (Bootstrap), AngularJS
- Backend: Python (Flask), SQLite
- Device Code: Arduino C++, Lua (NodeMCU)
- Web Hosting: Flask + WSGI
- API: RESTful with Flask Blueprints

---

## 📁 Project Structure

smart-energy-monitoring-system/
├── EdgeDevice/
│ ├── arduino/ # Arduino sketch (.ino)
│ └── nodemcu/ # NodeMCU sketch + embedded UI (HTML + AngularJS)
├── WebApp/
│ ├── sems/ # Flask backend (API, routes, models)
│ ├── static/ # AngularJS frontend files
│ ├── requirements.txt # Python dependencies
│ └── sems.py # Main app entry point
├── LICENSE
└── README.md


---

## 🚀 Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/smart-energy-monitoring-system.git
cd smart-energy-monitoring-system/WebApp
2. Install Backend Dependencies
Make sure you have Python 3 installed, then:

bash
Copier
Modifier
pip install -r requirements.txt
3. Run the Flask WebApp
bash
Copier
Modifier
python sems.py
Access the app at http://localhost:5000/

4. Flash NodeMCU/Arduino Code
Use the Arduino IDE or ESP8266 uploader to flash the code from /EdgeDevice/

Configure your Wi-Fi credentials in the NodeMCU sketch
