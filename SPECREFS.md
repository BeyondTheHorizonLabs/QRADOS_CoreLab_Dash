# QRADOS CoreLab Dash - Specification References (SPECREFS)

## Overview
This document outlines the key specifications, reference materials, and technical requirements for the **QRADOS CoreLab Dash** system.

## 1. System Architecture
- **Framework:** Node.js (Backend), React.js (Frontend)
- **Database:** PostgreSQL (Primary), JSON-based Log Storage (Secondary)
- **Communication Protocols:** WebSockets (Real-time Streaming), REST API (Data Retrieval)
- **Deployment:** Docker-based with `docker-compose`
- **Supported Platforms:** macOS, Linux, Windows (via WSL)

## 2. Hardware Specifications
- **Primary Computing Unit:** Raspberry Pi 5 / x86-64 Linux Server
- **Power Supply:** 48V 600W PSU (configurable)
- **Sensors:**
  - Electromagnetic Field (EMF) Sensors
  - RF Spectrum Analyzer (HackRF / RTL-SDR)
  - Ultrasonic Microphone Array
  - Optical Spectrum Analyzer
  - Temperature, Humidity, and Pressure Sensors
  - GPS & Magnetometer for Geospatial Logging

## 3. Software Components
### Backend API
- **Node.js v22**
- **Express.js for REST API**
- **Socket.io for real-time streaming**
- **PostgreSQL with TimescaleDB extension**
- **Data Encryption & Logging (Graylog, Loki)**

### Frontend Dashboard
- **React.js (Next.js-based UI)**
- **Chart.js for Data Visualization**
- **Tailwind CSS for Styling**
- **Location Selector for Planetary/Star System Mapping**

## 4. QRADOS Symbol Notations
The system uses **QRADOS (𝒬𝓡) Energy Notation** based on **field resonance and anomaly magnitude**:

- **𝒬𝓡 = B ⋅ A / V**
  - **B:** Magnetic Field Strength (T)
  - **A:** Electromagnetic Flux Area (m²)
  - **V:** Resonance Chamber Volume (m³)

## 5. Supported Testing Environments
- **Ground-Based:** Indoor & Outdoor Paranormal/UAP Field Testing
- **Aerospace & Astrophysics:** Future extension for planetary & deep-space anomaly detection
- **Laboratory Simulations:** AI-driven anomaly pattern recognition & signal analysis

## 6. API Reference
### Example Sensor Data Log Format
```json
{
  "timestamp": "2025-01-30T12:45:00Z",
  "device_id": "QRADOS-01",
  "sensor_type": "EMF",
  "value": 35.2,
  "unit": "µT",
  "status": "NORMAL",
  "location": "Earth-Lab"
}
```

## 7. Future Enhancements
- Integration with AI-based anomaly detection models
- Expansion of sensor array for multi-spectrum scanning
- Secure cloud storage for long-term data analysis
- QRADOS networking with distributed sensor nodes


