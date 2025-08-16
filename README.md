# HeaterControlSystem
ESP32-based heater controller with DS18B20 temperature sensor, buzzer, and LED alerts.
# ESP32 Heater Controller System

## Overview
This project implements a heater controller using an ESP32 and a DS18B20 digital temperature sensor. The system operates across multiple states: IDLE, HEATING, STABILIZING, TARGET REACHED, and OVERHEAT. Visual and audible indicators (LED and buzzer) are included to ensure safe operation.

## Features
- State-based temperature control
- LED blinking during heating
- Overheat protection with buzzer + LED alert
- Serial monitor output for debugging
- Easily extendable for future enhancements

## Hardware
- ESP32 Development Board
- DS18B20 Temperature Sensor
- Buzzer
- Two LEDs
- Resistors

## Connections
- DS18B20 → GPIO15
- Heater LED → GPIO4
- Buzzer → GPIO5
- Alert LED → GPIO2

## How to Run
1. Create a new project on Wokwi and select ESP32
2. Install libraries: OneWire, DallasTemperature
3. Upload `HeaterControlSystem.ino'
4. Observe state transitions as temperature changes

## Block Diagram
<img width="735" height="361" alt="image" src="https://github.com/user-attachments/assets/31b76eca-c7d1-470c-99a4-e5952fdb66ac" />


## Wokwi Simulation
https://wokwi.com/projects/439337980792678401

## Future Enhancements
- Multiple heating profiles
- Data logging
- BLE/Wi-Fi monitoring
- PID control
