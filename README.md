# Smart Knee Exoskeleton using ESP32 and MPU6050

## Overview

This project presents the design and development of a Smart Knee Exoskeleton that assists users during walking, standing, and sitting activities. The system is built around the ESP32 microcontroller and utilizes an MPU6050 IMU sensor to monitor leg movement in real time. Based on the detected motion, a high-torque MG996R servo motor provides mechanical assistance to reduce strain on the knee joint.

The exoskeleton features Bluetooth Low Energy (BLE) connectivity, allowing users to monitor and control the system through a Progressive Web Application (PWA). Additional functionalities include OLED-based real-time diagnostics, battery monitoring, safety alerts, manual and automatic operating modes, and emergency SOS support.

---

## Project Objectives

- Provide mechanical assistance for knee movement during walking and standing.
- Detect leg motion using the MPU6050 sensor.
- Enable real-time monitoring through an OLED display.
- Allow wireless control through a BLE-based web application.
- Monitor battery status and ensure safe operation.
- Develop a lightweight and portable assistive mobility solution.

---

## Hardware Components

- ESP32 Development Board
- MPU6050 IMU Sensor
- MG996R High-Torque Servo Motor
- SSD1306 OLED Display
- XL4016 Buck Converter
- 7.4V Li-ion Battery Pack
- Buzzer
- LEDs (Status Indicators)
- Push Button
- Toggle Switch
- Connecting Wires and Mechanical Frame

---

## Software and Tools Used

- Arduino IDE
- Embedded C/C++
- ESP32 BLE Libraries
- Adafruit SSD1306 Library
- Adafruit GFX Library
- ESP32Servo Library
- Progressive Web Application (PWA)
- HTML, CSS, JavaScript

---

## System Architecture

<img src="https://github.com/SujalPatil1616/Smart-Knee-Exoskeleton-using-ESP32/blob/main/Block%20Diagram.png" width="700">

The ESP32 acts as the central controller of the system. Motion data from the MPU6050 sensor is continuously processed to determine the user's leg movement and posture. Based on the detected motion, the ESP32 controls the MG996R servo motor to provide assistive torque. The OLED display presents real-time system information, while Bluetooth communication enables wireless monitoring and control through the web application.

---

## Hardware Prototype

<img src="https://github.com/SujalPatil1616/Smart-Knee-Exoskeleton-using-ESP32/blob/main/Hardware.png" width="500">

The prototype consists of an ESP32-based control unit mounted on a wearable knee support structure. The servo mechanism provides controlled knee assistance, while sensors continuously monitor movement and system status.

---

## Web Application Dashboard

### Dashboard Interface

<img src="https://github.com/SujalPatil1616/Smart-Knee-Exoskeleton-using-ESP32/blob/main/app1.png" width="700">

<img src="https://github.com/SujalPatil1616/Smart-Knee-Exoskeleton-using-ESP32/blob/main/app2.png" width="700">

The Progressive Web Application (PWA) enables:

- Bluetooth connection to ESP32
- Manual and Automatic modes
- Real-time angle monitoring
- Battery voltage monitoring
- Servo angle control
- Speed adjustment
- Sensitivity adjustment
- Activity monitoring
- Emergency controls

---

## Working Principle

The MPU6050 sensor continuously measures the orientation and movement of the user's leg using its accelerometer and gyroscope. The ESP32 processes this information and determines whether the user is standing, walking, or sitting.

In Automatic Mode, the controller automatically calculates the required assistance and drives the MG996R servo motor to support knee movement. When the user attempts to stand up, the servo provides additional torque to reduce physical effort. During walking, the system adjusts the assistance according to the detected leg angle and movement pattern.

In Manual Mode, the user can directly control the servo position and operating parameters through the Bluetooth-enabled web application. The OLED display continuously shows important information such as operating mode, battery status, and sensor readings.

The battery monitoring system continuously checks the supply voltage and activates warning indications through LEDs and a buzzer whenever low battery conditions are detected. This ensures reliable and safe operation of the exoskeleton.

---

## Features

- Smart Walking Assistance
- Sit-to-Stand Support
- Real-Time Motion Detection
- Bluetooth Low Energy Communication
- Progressive Web Application Control
- OLED Diagnostic Dashboard
- Battery Voltage Monitoring
- Buzzer-Based Safety Alerts
- LED Status Indicators
- Manual and Automatic Operating Modes
- Adjustable Servo Speed
- Adjustable Assistance Sensitivity
- Persistent Settings Storage using ESP32 Preferences

---

## Code Features

The firmware includes:

- BLE Server Implementation
- BLE Command Handling
- MPU6050 Sensor Interfacing
- Servo Motor Control
- OLED Display Management
- Battery Monitoring System
- Safety and Alert Management
- EEPROM/Preferences Storage
- Auto and Manual Mode Switching
- Device Self-Test During Startup

---

## Results

### Manual Mode

The user can directly control the servo angle and operating parameters through the Bluetooth dashboard

### Automatic Mode

The system automatically detects user movement and provides assistive torque without manual intervention.

---

## Advantages

- Lightweight and Portable Design
- Real-Time Motion Assistance
- Wireless Monitoring and Control
- Low-Cost Implementation
- User-Friendly Interface
- Improved Mobility Support
- Safe and Reliable Operation
- Expandable IoT-Based Architecture

---

## Applications

- Rehabilitation Systems
- Physiotherapy Assistance
- Elderly Mobility Support
- Knee Weakness Assistance
- Wearable Robotics
- Medical Assistive Devices
- Smart Healthcare Systems
- Human Augmentation Research

---

## Future Scope

- Machine Learning-Based Gait Analysis
- Cloud-Based Health Monitoring
- Dual-Leg Synchronization
- Solar-Assisted Charging
- Mobile Application Integration
- Advanced Motion Prediction Algorithms
- Voice-Controlled Operation
- Enhanced Actuator Mechanisms

---

## Project Demonstration

The following video demonstrates the working of the Smart Knee Exoskeleton system, including manual control, automatic assistance mode, and Bluetooth-based operation.

[▶ Watch Demo](demo.mp4)https://github.com/SujalPatil1616/Smart-Knee-Exoskeleton-using-ESP32/blob/main/demo.mp4

## Conclusion

The Smart Knee Exoskeleton demonstrates the integration of embedded systems, sensor technology, wireless communication, and assistive robotics into a single wearable platform. By combining ESP32-based control, MPU6050 motion sensing, BLE connectivity, and servo-assisted mobility, the system provides an effective solution for mobility enhancement, rehabilitation support, and human-assistive applications.
