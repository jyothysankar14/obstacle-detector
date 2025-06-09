# ESP32/ESP8266 Obstacle Avoiding Bot with Blynk

This project uses an **ESP32** or **ESP8266**, an **IR sensor**, and the **Blynk IoT app** to control and monitor a basic obstacle-avoiding robot. When no obstacle is detected, the bot moves forward. If an obstacle is detected, it stops. Notifications are sent via Blynk.

## Features
- IR sensor-based obstacle detection
- Motor control using GPIO pins
- WiFi-enabled notification using Blynk
- Compatible with ESP32 and ESP8266 boards

## Components Required
- ESP32 or ESP8266 Dev Board
- IR Sensor Module
- L298N Motor Driver
- 2 DC Motors
- Jumper Wires
- Power Supply (Battery or USB)

## Circuit Diagram
**(See wiring_diagram.png)**

## Wiring

### For ESP32
| ESP32 Pin | Component         | Description            |
|-----------|------------------|------------------------|
| D21       | IR Sensor OUT    | Reads digital output   |
| GND       | IR Sensor GND    | Ground connection      |
| 3.3V      | IR Sensor VCC    | Powers the sensor      |
| D4        | Motor Driver IN1 | Motor control          |
| D5        | Motor Driver IN2 | Motor control          |
| D18       | Motor Driver IN3 | Motor control          |
| D19       | Motor Driver IN4 | Motor control          |
| GND       | Motor Driver GND | Common ground          |
| 5V/Battery| Motor Driver VCC | Motor power supply     |

### For ESP8266 (NodeMCU)
| ESP8266 Pin | Component         | Description            |
|-------------|------------------|------------------------|
| D4          | IR Sensor OUT    | Reads digital output   |
| GND         | IR Sensor GND    | Ground connection      |
| 3.3V        | IR Sensor VCC    | Powers the sensor      |
| D0          | Motor Driver IN1 | Motor control          |
| D1          | Motor Driver IN2 | Motor control          |
| D2          | Motor Driver IN3 | Motor control          |
| D3          | Motor Driver IN4 | Motor control          |
| GND         | Motor Driver GND | Common ground          |
| VIN/Battery | Motor Driver VCC | Motor power supply     |


## How to Run
1. Replace `YourAuthToken`, `YourWiFiSSID`, and `YourWiFiPassword` in the code.
2. Upload the code to your ESP32 or ESP8266 using Arduino IDE.
3. Open Blynk app, add a device and enable notifications.
4. Power up your bot and watch it go!

## License
This project is open-source under the MIT License.
"# obstacle-detector" 
