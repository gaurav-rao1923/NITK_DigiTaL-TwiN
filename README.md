# 🌡️ Real-Time IoT Temperature & Humidity Visualization in Unity

This project is a cross-platform **Unity application** that visualizes real-time and predicted **temperature and humidity** data from **NodeMCU ESP8266 + DHT11 sensors**. It provides a 3D interactive environment with visual cues, color-coded heat zones, and predictive insights for intelligent environmental monitoring.

---

## 🚀 Features

- 🔴 **Real-Time 3D Visualization** of temperature & humidity data  
- 📡 **MQTT Integration** for live sensor updates from 7 nodes  
- 🌈 **Color-coded ceilings** based on temperature:  
  - **< 32°C** → Blue  
  - **32–35°C** → Light Red  
  - **> 35°C** → Dark Red  
- 🧊 **Glass-like ceiling material** with visual effects  
- 📈 **Firebase** for storing historical data  
- 🤖 **Machine Learning** prediction of future temperature/humidity  
- 🖱️ **Click/Tap to Inspect** rooms and corridors (shows real-time values)  
- 📊 Dual chart system:  
  - Real-time data  
  - Predicted data  
- 💻📱 **Cross-platform** build support: Windows, Android, iOS  

---

## 🧱 Architecture

- **Unity (C#)** — 3D interface, interaction, MQTT client, animation  
- **MQTT (Mosquitto)** — lightweight message broker for IoT sensor data  
- **NodeMCU ESP8266 + DHT11** — data collection (temperature, humidity)  
- **Python** — MQTT-to-Firebase bridge  
- **Firebase Realtime DB** — cloud storage for sensor + prediction data  
- **ML Model** — forecasts temperature/humidity for user-selected dates  

---

## 📁 Project Structure

##├── Assets/ ## All Unity assets (scripts, scenes, prefabs)
##├── Packages/ ## Unity package manager settings
##├── ProjectSettings/ ## Unity editor settings
##├── .gitignore ## Files/folders excluded from version control
##└── README.md ## Project documentation (this file)

yaml
Copy
Edit

---

## ⚙️ Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/your-repo-name.git
2. Open the Project in Unity
Use Unity Editor 2021.3 or later

Open the folder containing Assets, Packages, and ProjectSettings

3. Set Up Your MQTT Environment
Connect your NodeMCU ESP8266 boards to DHT11 sensors

Make sure they publish temperature and humidity data to MQTT topics

Use Mosquitto or another broker as your MQTT server

4. Run the Python MQTT-to-Firebase Script
A Python script subscribes to MQTT and pushes data to Firebase

Use paho-mqtt and firebase-admin Python packages

5. Launch the Unity Scene
Press Play in Unity

The ceiling changes color based on live temperature data

Tap/click objects to display location, temperature, and humidity

🧠 ML Prediction Module
Data is stored in Firebase

ML model (e.g., LSTM or regression) predicts temperature/humidity for a selected date

Unity queries Firebase and displays the predicted values with the same color rules

Prediction charts appear alongside real-time data charts

🛠️ Tools & Technologies
Unity (C#)

NodeMCU ESP8266 + DHT11

MQTT (Mosquitto)

Python (MQTT → Firebase bridge)

Firebase Realtime Database

TensorFlow / Scikit-learn (for ML predictions)

📌 Future Enhancements
🔔 Add visual/audio alerts when thresholds are crossed

🕶️ VR/AR integration for immersive visualization

🧾 Historical data explorer with trend lines

🎨 Better UX with dashboards and filter options

🤝 Contributing
Pull requests are welcome!
Please open an issue to discuss your ideas or proposed changes.

📜 License
This project is open-source and licensed under the MIT License.

🙏 Acknowledgments
Unity Technologies

Firebase by Google

Eclipse Mosquitto MQTT Broker

Open Source DHT11 & ESP8266 community

OpenAI ChatGPT (for architecture & documentation assistance 😄)
