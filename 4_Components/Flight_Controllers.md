# 🎮 Flight Controllers (FC)

A **flight controller (FC)** is the central unit that controls the drone's flight behavior by processing data from sensors and executing stabilization algorithms in real time.

---

## 🧠 Core Functions:
- **Stabilization:** Uses IMU (gyroscope + accelerometer) to balance the drone
- **Command interpretation:** Processes inputs from RC or mission planner
- **Motor output control:** Sends signals to ESCs to adjust propeller speeds
- **Sensor fusion:** Combines GPS, barometer, magnetometer, etc.
- **Autonomous flight:** Executes missions with GPS waypoints and failsafes

---

## 🧩 Internal Sensors:
| Sensor | Function |
|--------|----------|
| Gyroscope | Measures angular velocity |
| Accelerometer | Detects tilt & motion |
| Magnetometer | Acts as a compass |
| Barometer | Measures altitude |
| GPS | Positioning and navigation |

---

## 🛠️ Popular Flight Controllers

| FC Name | Supported Software | Use Case |
|--------|---------------------|----------|
| **Pixhawk** | PX4, ArduPilot | Research, mapping, long-range |
| **Betaflight F4/F7** | Betaflight | FPV racing, freestyle |
| **Kakute F7** | INAV, Betaflight | Mid-level freestyle builds |
| **DJI Naza-M** | DJI Assistant | Commercial photography drones |

---

## 🔌 Connectivity
- USB for setup & firmware
- UART for GPS, telemetry, camera, etc.
- PWM outputs to ESCs

---
