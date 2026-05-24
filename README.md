# 🚗 Vision-Guided Autonomous Vehicle

IoT project carried out at Icam (2025–2026) — a mobile vehicle prototype 
able to reach a target zone inside an arena while avoiding obstacles, 
**without using a single on-board sensor**.

All the intelligence sits off the vehicle: a fixed camera mounted at head 
height (150–177 cm) films the scene, and a Raspberry Pi 3 processes the 
video stream in real time using OpenCV to locate the vehicle, detect 
obstacles and identify the finish line. Movement commands are then sent 
over Wi-Fi to an ESP32, which drives the DC motors through an L298N driver.

The approach draws inspiration from real-world problems found in 
teleoperated robotics and centralized surveillance systems, and opens up 
a broader reflection on inclusive applications — particularly driving 
assistance for visually impaired people.

## ✨ Project highlights
- **No on-board sensors** — everything relies on external vision
- **Real-time processing** on a Raspberry Pi 3 (tight performance constraints)
- **Safety logic** — the car stops automatically on signal or vision loss
- **Live visualization** of the computed trajectory
- **Logging system** to replay and analyze each run
- **Tight budget** — under €200
- **Agile workflow** — the project lead role rotates between team members

## 🎯 Requirements (summary)
- Flat arena, 2 to 3 m²
- Full run completed in under 10 minutes
- Secure Wi-Fi communication
- Battery life sufficient to chain multiple test runs
- Obstacles randomized between runs
