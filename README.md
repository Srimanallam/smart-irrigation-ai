<p align="center">
  <img src="https://img.shields.io/badge/IoT-ESP32-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Backend-FastAPI-green?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Dashboard-Streamlit-red?style=for-the-badge" />
  <img src="https://img.shields.io/badge/AI-CNN-orange?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Status-Active-brightgreen?style=for-the-badge" />
</p>
 AI-Powered Smart Irrigation & Crop Health Monitoring  
ESP32 + MQTT + FastAPI + Streamlit + TensorFlow
A complete end-to-end IoT + AI system that monitors soil conditions, automates irrigation, and detects plant diseases using a CNN model.
## Architecture Overview
      ┌──────────┐       MQTT        ┌─────────────┐
      │  ESP32   │ ─────────────────▶│   Backend    │
      │ Soil/DHT │                  │  (FastAPI)   │
      └──────────┘◀─────────────────│ MQTT Consumer│
         ▲   │     Pump Control      └─────────────┘
         │   │                             │
         │   └─────────────────────────────┘
         │                             REST API
         ▼                                  │
    ┌─────────┐                       ┌─────────────┐
    │  Relay   │                       │ Streamlit   │
    │  Pump    │◀──────────────────────│  Dashboard  │
    └─────────┘                       └─────────────┘
    




