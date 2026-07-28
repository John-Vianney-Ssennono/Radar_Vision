# Smart Radar Glasses for Visually Impaired Navigation 👓📡

![Platform](https://img.shields.io/badge/Platform-Arduino%20UNO-blue)
![Category](https://img.shields.io/badge/Category-Assistive%20Technology-green)
![Status](https://img.shields.io/badge/Status-Prototype-orange)

An electronic assistive wearable designed to aid visually disadvantaged individuals. Using ultrasonic detection integrated directly into a pair of glasses, the device continuously scans the wearer's forward path to detect nearby obstacles and provides immediate real-time audio feedback to prevent collisions.

---

## 📌 Project Overview

Navigating unfamiliar or dynamic environments can pose significant safety challenges for individuals with visual impairments. These **Radar Vision Glasses** act as a hands-free proximity sensor. Mounted onto the frame, an ultrasonic transmitter/receiver emits high-frequency sound waves to measure distance. When an obstacle is detected within range, a integrated active buzzer alerts the wearer to stop or alter their path.

---

## 🛠️ Hardware & Pin Configuration

The system is powered by an **Arduino UNO** control module. Below is the precise pin-mapping derived from the hand design schematics:

| Component | Component Pin | Arduino UNO Pin | Function / Wire Description |
| :--- | :--- | :--- | :--- |
| **Arduino UNO** | `5V` | `5V [Power]` | System power line |
| **Arduino UNO** | `GND` | `GND` | Common ground connection |
| **Active Buzzer (Buz 1)** | `+` (Positive) | **Digital Pin 4** | Audio alert trigger |
| **Active Buzzer (Buz 1)** | `-` (Ground) | **GND** | Ground |
| **Ultrasonic Sensor (ULT-SENSOR-1)** | `VCC` | **5V** | 5V Power Supply |
| **Ultrasonic Sensor (ULT-SENSOR-1)** | `Trig` (Sender) | **Digital Pin 10** | Ultrasonic pulse trigger output |
| **Ultrasonic Sensor (ULT-SENSOR-1)** | `Echo` (Receiver)| **Digital Pin 11** | Echo pulse width receiver input |
| **Ultrasonic Sensor (ULT-SENSOR-1)** | `GND` | **GND** | Ground |

---

## 📐 Mechanical & Wearable Design

The system integrates electronic control directly onto a standard eyeglass frame structure:
