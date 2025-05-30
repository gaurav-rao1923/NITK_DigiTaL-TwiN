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

