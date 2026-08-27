# Home Automation Using ESP32 & Blynk

---

## 📌 Project Overview

This project implements a Smart Home Automation System using ESP32, Blynk IoT Platform, and a 4-Channel Relay Module. The system allows users to control household appliances remotely through the Blynk mobile application as well as manually using physical push buttons.

The ESP32 connects to a Wi-Fi network and communicates with the Blynk Cloud. Users can switch appliances ON/OFF from anywhere using a smartphone, while the relay module controls the actual electrical loads.

The complete system is developed using Arduino IDE and tested using the Blynk IoT platform.

---

## 🛠️ Tools & Technologies
- ESP32
- Arduino IDE
- Blynk IoT Platform
- Embedded C/C++
- Wi-Fi Communication
- 4-Channel Relay Module
- Push Buttons

---

## 🧩 Main Components
1. ESP32 Controller

The ESP32 acts as the central controller of the system. It receives commands from the Blynk Cloud and controls the connected relays.

2. Blynk IoT Platform

Blynk provides a mobile dashboard that allows users to control appliances remotely using virtual buttons.

Smartphone → Blynk Cloud → ESP32

3. Relay Module

The relay module acts as an electronic switch that controls electrical appliances.

ESP32 → Relay → Appliance

4. Push Buttons

Push buttons provide manual control of appliances without using the mobile application.

Push Button → ESP32 → Relay

---

## 🔌 System Architecture
```text
       Smartphone
                │
                │
          Blynk Cloud
                │
            Wi-Fi
                │
             ESP32
      ┌────────┼────────┐
      │        │        │
   Relay1   Relay2   Relay3   Relay4
      │        │        │        │
   Load1    Load2    Load3    Load4

      ↑
Push Buttons
```
---

## ⚙️ Pin Configuration

```text
Relay Pins
Relay	GPIO
Relay 1	GPIO 2
Relay 2	GPIO 12
Relay 3	GPIO 14
Relay 4	GPIO 27

Push Button Pins
Button	GPIO
Button 1	GPIO 26
Button 2	GPIO 25
Button 3	GPIO 33
Button 4	GPIO 32
```
---

## 🔄 Working Principle
- ESP32 connects to the Wi-Fi network.
- ESP32 connects to Blynk Cloud using the authentication token.
- User presses a button on the Blynk App.
- Blynk sends the command to ESP32.
- ESP32 activates the corresponding relay.
- The relay switches the connected appliance ON/OFF.
- Push buttons can also manually control the relays.
- Relay status is synchronized with the Blynk dashboard.

---

## 📱 Blynk Dashboard

The dashboard contains four virtual switches:

V1 → Relay 1

V2 → Relay 2

V3 → Relay 3

V4 → Relay 4

Each switch controls one appliance.

---

## 🚀 Features

- Remote appliance control using smartphone
- Wi-Fi based communication
- Four-channel relay control
- Manual push-button operation
- Real-time synchronization
- Low-cost IoT solution
- User-friendly interface

---

## 📊 Communication Flow
```text
Mobile App
     ↓
Blynk Cloud
     ↓
Wi-Fi
     ↓
ESP32
     ↓
Relay Module
     ↓
Electrical Appliance
```
