# Adaptive Cruise Control (ACC) Simulation Project

## Project Overview

This project simulates an **Adaptive Cruise Control (ACC) system** using Arduino. The system automatically detects obstacles and emergency tilts and reacts by activating a relay and a buzzer to maintain safety.

## Aim

To simulate an ACC system that **automatically detects obstacles and emergencies** and **reacts to maintain a safe distance** from objects ahead.

## Components Used

* **Arduino Uno R3**: Main controller that reads sensors and controls outputs.
* **IR-08H Obstacle Sensor**: Detects objects in front.
* **Tilt Sensor**: Detects sudden tilts or movements (simulates emergencies).
* **Relay Module**: Simulates braking or throttle.
* **Buzzer**: Sounds an alert when danger is detected.
* **Breadboard**: Connects components safely.
* **Jumper Wires**: Connects components to Arduino.
* **USB Cable**: Powers Arduino and uploads code.

## Component Functions

* **IR Sensor**: Detects objects ahead and triggers relay and buzzer.
* **Tilt Sensor**: Detects if the sensor is tilted and triggers the system.
* **Relay**: Turns ON to simulate brakes when sensors are triggered.
* **Buzzer**: Beeps for 2 seconds when sensors are triggered.

## Connections

* **IR Sensor**: VCC → 5V, GND → GND, OUT → D2
* **Tilt Sensor**: Pin1 → D3, Pin2 → GND
* **Relay Module**: IN → D5, VCC → 5V, GND → GND
* **Buzzer**: + → D4, – → GND
* **Power/Ground**: 5V and GND from Arduino to breadboard

## Working Principle

1. The **IR sensor** detects objects in front.
2. The **tilt sensor** detects sudden tilts or movement.
3. When either sensor is triggered, the **Arduino turns ON the relay and buzzer for 2 seconds**.
4. After 2 seconds, both the relay and buzzer turn off, ready for the next detection.

## Testing Steps

1. Connect all components according to the connections table.
2. Upload the Arduino code.
3. Test **IR sensor**: bring an object close → relay clicks + buzzer sounds.
4. Test **tilt sensor**: tilt it → relay clicks + buzzer sounds.
5. Observe system responding to both sensors correctly.

## Notes

* Both **relay and buzzer activate for 2 seconds** when a sensor is triggered.
* The system demonstrates the **core concept of ACC** without using real car hardware.

## Author

[LUTWAMA JOEL MARTHAN]

## Date

[Date of Project]
