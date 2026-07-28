# Smart Radar Vision Glasses for Assistive Navigation 👓📡

![Platform](https://img.shields.io/badge/Platform-Arduino%20Uno%20R3-blue)
![Category](https://img.shields.io/badge/Category-Assistive%20Technology-green)
![Status](https://img.shields.io/badge/Status-Static%20Sensor%20Prototype-orange)

An electronic assistive wearable designed to aid visually disadvantaged individuals by detecting obstacles and preventing collisions in real time. Mounted directly onto a pair of glasses, this system uses ultrasonic distance sensing to continuously monitor the wearer's path and provide immediate audio feedback via a buzzer.

---

## 📌 Project Overview

For individuals with visual impairments, detecting obstacles at head or chest level can be challenging with traditional tools. These **Radar Vision Glasses** serve as a hands-free proximity scanner. 

Unlike motorized radar systems that rely on servo sweeps, this streamlined prototype utilizes a **fixed, hand-directed ultrasonic sensor** mounted to the eyeglass frame. The wearer manually scans their environment by moving their head, allowing for direct, real-time spatial awareness without the added weight, noise, or power draw of a servo motor.

---

## 🛠️ Hardware Setup & Pin Mapping

The circuit is controlled by an **Arduino Uno R3**. All components are wired according to the optimized schematic layout below:

| Component | Component Pin | Arduino Uno Pin | Function / Description |
| :--- | :--- | :--- | :--- |
| **Arduino Uno R3** | `5V` | `5V` | System 5V Power Line |
| **Arduino Uno R3** | `GND` | `GND` | Common Ground |
| **HC-SR04 Ultrasonic Sensor** | `VCC` | `5V` | 5V Power Supply |
| **HC-SR04 Ultrasonic Sensor** | `Trig` | **Digital Pin 8** | Ultrasonic Pulse Trigger Output |
| **HC-SR04 Ultrasonic Sensor** | `Echo` | **Digital Pin 9** | Echo Pulse Receiver Input |
| **HC-SR04 Ultrasonic Sensor** | `GND` | `GND` | Ground |
| **Active Buzzer** | `+` (Positive) | **Digital Pin 4** | Audio Alert Output Signal |
| **Active Buzzer** | `-` (Ground) | `GND` | Ground |

---

## 📐 Wearable Design & Mechanical Integration

The components are integrated onto a standard eyeglass frame to keep the wearable lightweight and comfortable:
