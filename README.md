# Automatic Water Level Controller using Arduino

This project demonstrates the creation of an Automatic Water Level Controller using Arduino, providing an efficient solution for managing water levels in tanks. It helps to prevent water wastage and ensures a consistent water supply through automation and user control features.

## Features

- **Automatic and Manual Modes:** Switch between automatic (level-based) control and manual override.
- **Water Level Display:** Shows real-time water level percentage on a 16x2 LCD.
- **Pump Control:** Automatically activates/deactivates the water pump according to set levels.
- **User Settable Threshold:** Allows setting the tank's maximum water level as a reference.
- **EEPROM Storage:** Remembers set level even after power loss.

## Components Required

- Arduino UNO/Nano
- Ultrasonic Sensor (HC-SR04 or similar)
- 16x2 LCD (with parallel interface)
- Relay Module (to control the water pump)
- Push Buttons (for mode and set operations)
- Jumper wires, Resistors, Breadboard

## Circuit Connections

| Arduino Pin | Component            |
|-------------|---------------------|
| 2,3,4,5,6,7 | LCD (RS,E,D4,D5,D6,D7) |
| 8           | Ultrasonic Trigger  |
| 9           | Ultrasonic Echo     |
| 10          | Set/Manual Button   |
| 11          | Mode Switch (Manual/Auto) |
| 12          | Relay Module (Pump) |

*Connect VCC/GND as needed for all modules.*

## Usage

1. **Upload the code to your Arduino.**
2. **Set Maximum Level:** In AUTO mode, press the SET button when the tank is full to set reference (max) level.
3. **Modes:** Use the MODE switch to toggle between AUTO and MANUAL.
4. **Manual Pump:** In MANUAL mode, pressing SET toggles the pump ON/OFF.
5. **The LCD shows water level (%) and pump status.**

## Code

See [`water_level_controller.ino`](water_level_controller.ino).

---
