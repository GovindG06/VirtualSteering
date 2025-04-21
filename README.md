#VirtualSteering
# Gesture-Based Virtual Steering System Using Hand Tracking

## 📌 Project Overview

This project is a gesture-controlled virtual steering system developed as part of the **Project-Based Learning (PBL)** curriculum in college. The system utilizes real-time hand tracking to simulate keyboard inputs for directional control, enabling an intuitive interface for navigation in simulation or gaming environments.

Leveraging computer vision and hand landmark detection, the system recognizes wrist movements captured via webcam and maps them to keyboard commands (`W`, `A`, `S`, `D`) to represent forward, backward, left, and right movements.

---

## 🎯 Objectives

- To implement a real-time hand gesture recognition system using a standard webcam.
- To translate hand movements into virtual keyboard inputs for directional control.
- To demonstrate integration of computer vision with hardware interfacing.

---

## 🛠️ Technologies Used

| Technology   | Purpose                                  |
|--------------|-------------------------------------------|
| Python       | Core programming language                 |
| OpenCV       | Real-time image capture and display       |
| MediaPipe    | Hand landmark detection and tracking      |
| ctypes (Windows) | Virtual keyboard input simulation     |

---

## 🧠 System Architecture

1. **Hand Detection**:  
   Utilizes MediaPipe to detect and track hand landmarks in real-time using webcam input.

2. **Gesture Interpretation**:  
   Calculates the relative positions and angles of the wrists to determine the intended direction.

3. **Keyboard Control**:  
   Sends simulated keystrokes using `ctypes.windll` to control movement:
   - `W` → Move forward
   - `S` → Move backward
   - `A` → Turn left
   - `D` → Turn right

---
