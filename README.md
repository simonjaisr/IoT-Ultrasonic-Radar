# ESP8266 Radar System

## Overview
An ultrasonic radar system that scans 180° and displays detected objects on a web interface in real-time.

## Features
- **180° Servo Rotation** using MG90S
- **Distance Measurement** with HC-SR04 ultrasonic sensor
- **Web Visualization** with live updating radar display
- **WiFi Connectivity** via ESP8266

## Components
| Component       | Purpose                     |
|-----------------|-----------------------------|
| ESP8266         | WiFi connectivity and control |
| MG90S Servo     | Rotates ultrasonic sensor   |
| HC-SR04         | Distance measurement        |
| 5V Power Supply | External power for servo    |

## How It Works
1. The servo rotates from 0° to 180° in increments
2. At each angle, the ultrasonic sensor measures distance
3. Distance data is sent to a web interface
4. Objects are plotted on a radar-style display

## Installation
### Prerequisites
- Arduino IDE with ESP8266 support
- Basic electronics knowledge

### Setup
1. **Hardware Connections**
   - Servo: Connect to D1
   - HC-SR04: Trig to D5, Echo to D6
   - Power servo with external 5V supply

2. **Software Upload**
   - Open `radar.ino` in Arduino IDE
   - Select board: "NodeMCU 1.0 (ESP-12E Module)"
   - Upload to ESP8266

3. **Access the Radar**
   - Connect to the ESP8266's WiFi network
   - Open the provided IP address in a web browser

## License
MIT License
