Home Automation Using ESP32 and Blynk
📌 Project Overview

The Home Automation System is an IoT-based smart home project developed using ESP32, 4-Channel Relay Module, Push Buttons, and the Blynk IoT Platform.

The system allows users to control home appliances remotely using the Blynk mobile application as well as manually using physical push buttons. The ESP32 connects to Wi-Fi and communicates with the Blynk Cloud to provide real-time control and monitoring.

🎯 Objectives
Control home appliances remotely using a smartphone.
Provide manual control through push buttons.
Enable real-time synchronization between hardware and mobile application.
Develop a low-cost smart home automation solution.
Utilize IoT technology for wireless appliance control.
⚙️ Components Required
Hardware
ESP32 Development Board
4-Channel Relay Module
4 Push Buttons
Wi-Fi Network
AC Bulbs/Loads
Jumper Wires
Breadboard/PCB
Power Supply
Software
Arduino IDE
Blynk IoT Platform
Embedded C/C++
ESP32 Board Package
🔌 Pin Configuration
Relay Connections
Relay	ESP32 Pin
Relay 1	GPIO 2
Relay 2	GPIO 12
Relay 3	GPIO 14
Relay 4	GPIO 27
Push Button Connections
Button	ESP32 Pin
Button 1	GPIO 26
Button 2	GPIO 25
Button 3	GPIO 33
Button 4	GPIO 32
Blynk Virtual Pins
Appliance	Virtual Pin
Relay 1	V1
Relay 2	V2
Relay 3	V3
Relay 4	V4
🧠 Working Principle
ESP32 connects to the Wi-Fi network.
ESP32 authenticates with the Blynk Cloud using the Auth Token.
User controls appliances through the Blynk mobile application.
Blynk sends commands to ESP32.
ESP32 switches the corresponding relay ON or OFF.
Physical push buttons can also control appliances locally.
Relay status is synchronized with the Blynk dashboard.
Real-time monitoring is available through the smartphone.
📡 System Architecture
        Smartphone
             │
             │
        Blynk Cloud
             │
             │ Wi-Fi
             │
           ESP32
      ┌──────┼──────┐
      │      │      │
   Relay1 Relay2 Relay3 Relay4
      │      │      │      │
   Load1  Load2  Load3  Load4

      ↑      ↑      ↑      ↑
 Push Button Inputs
🚀 Features
Remote appliance control through Blynk App
Manual control using push buttons
Real-time status synchronization
Wi-Fi based communication
Low-cost implementation
Easy installation
Expandable architecture
Smart home automation
📱 Blynk Dashboard

The Blynk dashboard contains:

Switch Widget for Relay 1 (V1)
Switch Widget for Relay 2 (V2)
Switch Widget for Relay 3 (V3)
Switch Widget for Relay 4 (V4)

Users can control appliances from anywhere using the internet.

🔄 Working Flow
Start
  ↓
Initialize ESP32
  ↓
Connect to Wi-Fi
  ↓
Connect to Blynk Cloud
  ↓
Wait for User Command
  ↓
Blynk App / Push Button
  ↓
Relay Control
  ↓
Appliance ON/OFF
  ↓
Update Blynk Dashboard
  ↓
Repeat
📊 Communication Method
Wi-Fi Communication

The ESP32 uses the built-in Wi-Fi module to communicate with Blynk Cloud.

ESP32 → Wi-Fi Router → Blynk Cloud → Smartphone
