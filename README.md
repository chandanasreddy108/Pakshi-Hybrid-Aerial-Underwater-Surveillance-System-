# 🦅 Pakshi – Hybrid Aerial & Underwater Surveillance System

<p align="center">

![Status](https://img.shields.io/badge/Status-Under%20Development-blue)
![Platform](https://img.shields.io/badge/Platform-Hybrid%20Drone%20%26%20ROV-success)
![Microcontroller](https://img.shields.io/badge/Controller-ESP32%20%7C%20Arduino-orange)
![License](https://img.shields.io/badge/License-MIT-green)

</p>

> **Pakshi** is a **hybrid surveillance robot** capable of operating both **in air and underwater**, designed for search & rescue, environmental monitoring, military reconnaissance, disaster response, and industrial inspections.

The project combines aerial mobility with underwater navigation into a single intelligent robotic platform, enabling seamless transition between air and water while performing real-time surveillance, sensing, and autonomous data collection.

---

# 📖 Table of Contents

- Overview
- Problem Statement
- Objectives
- Key Features
- Applications
- System Architecture
- Hardware Components
- Software Stack
- Working Principle
- Repository Structure
- Installation
- Future Improvements
- Development Roadmap
- Contributors
- License

---

# 🌍 Overview

Traditional drones cannot perform underwater inspection, while underwater ROVs cannot perform aerial reconnaissance.

**Pakshi** bridges this gap by integrating both capabilities into one robotic platform.

The system can:

- Fly over inaccessible areas
- Land on water
- Dive underwater
- Collect images and sensor data
- Return to the surface
- Continue aerial operation

This hybrid capability makes Pakshi suitable for numerous real-world applications where both aerial and underwater intelligence are required.

---

# ❗ Problem Statement

Current surveillance systems are limited to a single operating environment.

- Aerial drones cannot inspect underwater structures.
- Underwater robots cannot rapidly relocate over long distances.
- Deploying separate systems increases operational cost and complexity.

Pakshi addresses these challenges through a unified hybrid robotic platform.

---

# 🎯 Objectives

- Design a dual-environment robotic platform
- Enable seamless transition between air and underwater modes
- Capture live video and sensor data
- Support autonomous navigation
- Reduce deployment cost using open-source hardware
- Develop a modular and scalable robotic architecture

---

# ✨ Key Features

## 🚁 Aerial Mode

- Stable quadcopter flight
- GPS navigation
- Altitude hold
- Waypoint navigation
- Manual and autonomous modes
- FPV camera streaming

---

## 🌊 Underwater Mode

- Thruster-based propulsion
- Waterproof electronics enclosure
- Depth monitoring
- Obstacle avoidance
- Underwater camera
- Environmental sensing

---

## 📡 Communication

- Wi-Fi
- ESP-NOW
- RF Control
- Telemetry
- GPS Tracking

---

## 🤖 Intelligent Functions

- Autonomous navigation
- Obstacle detection
- Sensor fusion
- Environmental monitoring
- Mission logging
- Live video transmission

---

# 🛠 Applications

- Coastal surveillance
- Search and rescue
- Flood inspection
- Bridge inspection
- Dam inspection
- Ship hull inspection
- Marine research
- Underwater exploration
- Military reconnaissance
- Environmental monitoring

---

# 🏗 System Architecture

```
                    Ground Station
                          │
        ┌─────────────────┴─────────────────┐
        │                                   │
   Live Telemetry                    Live Video
        │                                   │
        └──────────────┬────────────────────┘
                       │
               Hybrid Controller
                       │
      ┌────────────────┼─────────────────┐
      │                │                 │
 Flight Controller   ESP32          Sensor Module
      │                │                 │
      │                │                 │
 Brushless Motors   Cameras      IMU • GPS • Pressure
      │                │                 │
      └────────────────┼─────────────────┘
                       │
              Underwater Thrusters
```

---

# 🔧 Hardware Components

## Flight System

- Brushless Motors
- ESCs
- Propellers
- Flight Controller
- Li-Po Battery

## Underwater System

- Waterproof Thrusters
- Waterproof Housing
- Pressure Sensor
- Depth Sensor

## Electronics

- ESP32
- Arduino Nano
- GPS Module
- IMU (MPU6050 / MPU9250)
- Camera Module
- Ultrasonic Sensor
- Power Distribution Board

---

# 💻 Software Stack

| Category | Technologies |
|-----------|--------------|
| Programming | C++, Python |
| IDE | Arduino IDE |
| Microcontroller | ESP32 |
| CAD | SolidWorks / Fusion 360 |
| Version Control | Git & GitHub |
| Communication | ESP-NOW, Wi-Fi |
| Flight Firmware | ArduPilot / PX4 *(planned)* |

---

# ⚙ Working Principle

### ✈️ Aerial Operation

- Takeoff
- GPS navigation
- Area surveillance
- Water landing

↓

### 🌊 Water Transition

- Motors stop
- Waterproof systems activate
- Thrusters engage

↓

### 🤿 Underwater Navigation

- Dive
- Capture images
- Collect environmental data
- Navigate around obstacles

↓

### 🚁 Surface Return

- Ascend
- Transition to flight mode
- Resume aerial surveillance

---

# 📂 Repository Structure

```
Pakshi/
│
├── Hardware/
│   ├── CAD Models
│   ├── PCB Design
│   ├── Schematics
│
├── Firmware/
│   ├── ESP32
│   ├── Arduino
│   ├── Sensors
│
├── Software/
│   ├── Ground Station
│   ├── Telemetry
│
├── Documentation/
│   ├── Images
│   ├── Circuit Diagrams
│   ├── Reports
│
├── Media/
│   ├── Photos
│   ├── Videos
│
└── README.md
```

---

# 🚀 Getting Started

## Clone Repository

```bash
git clone https://github.com/koushikmvkk-gif/Pakshi-Hybrid-Aerial-Underwater-Surveillance-System-.git
```

---

## Open Firmware

Open the Arduino sketches located in:

```
Firmware/
```

---

## Upload

Select the appropriate board:

- ESP32
- Arduino Nano

Upload the firmware.

---

## Assemble Hardware

- Connect sensors
- Install thrusters
- Mount motors
- Waterproof the electronics
- Calibrate IMU
- Test communication

---

# 📈 Development Roadmap

- [x] Initial Concept Design
- [x] Hybrid Architecture Planning
- [ ] Mechanical Design
- [ ] Waterproof Enclosure
- [ ] Flight Control Integration
- [ ] Underwater Propulsion
- [ ] Camera System
- [ ] Autonomous Navigation
- [ ] AI Object Detection
- [ ] Mission Planner Integration
- [ ] Field Testing
- [ ] Final Prototype

---

# 🔮 Future Improvements

- AI-based object detection
- Autonomous underwater mapping
- SLAM navigation
- Multi-camera vision system
- Sonar imaging
- Thermal camera integration
- Underwater robotic arm
- Swarm communication
- Edge AI processing
- Cloud mission logging

---

# 📊 Project Status

| Module | Status |
|---------|--------|
| Mechanical Design | 🟡 In Progress |
| Electronics | 🟡 In Progress |
| Firmware | 🟡 In Progress |
| Flight System | 🔲 Planned |
| Underwater System | 🔲 Planned |
| AI Features | 🔲 Planned |
| Documentation | 🟢 Active |

---

# 🤝 Contributing

Contributions are welcome!

If you'd like to improve this project:

1. Fork the repository
2. Create a new branch

```bash
git checkout -b feature-name
```

3. Commit your changes

```bash
git commit -m "Added new feature"
```

4. Push your branch

```bash
git push origin feature-name
```

5. Open a Pull Request

---

# 👨‍💻 Author

**Koushik M** <br>
**Chandana S**

**Mechatronics Engineering Student**  
The Oxford College of Engineering, Bengaluru

**Areas of Interest**

- Robotics
- Embedded Systems
- Edge AI
- UAV Systems
- Autonomous Vehicles
- Underwater Robotics
- IoT

---

# ⭐ Support

If you found this project useful, consider giving it a **⭐ Star** on GitHub!

It helps others discover the project and motivates future development.

---

# 📜 License

This project is licensed under the **MIT License**.

Feel free to use, modify, and contribute while providing appropriate attribution.

---

## 🚀 "One Robot. Two Worlds. Unlimited Possibilities."
