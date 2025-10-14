# Arduino-Based Obstacle Avoiding and Bluetooth-Controlled Car

This project demonstrates an autonomous robot car that can detect and avoid obstacles using an ultrasonic sensor and can also be manually controlled via a Bluetooth-enabled smartphone.  
It combines basic robotics, sensors, and communication modules to show how embedded systems can be used to create an intelligent vehicle.

![Arduino Car](https://github.com/user-attachments/assets/c27c8bec-e221-4983-9888-02f36ac786ff)

---

## Project Overview

The robot car is powered by an Arduino Uno microcontroller and uses an ultrasonic sensor (HC-SR04) to measure distance from obstacles.  
When the sensor detects an object within a certain range, the Arduino automatically stops or changes the car’s direction to avoid a collision.  

The car also includes an HC-05 Bluetooth module that allows wireless control using an Android smartphone app.  
This makes it possible to drive the robot manually or let it operate autonomously in obstacle avoidance mode.

---

## Components and Tools Used

| Component | Description |
|------------|-------------|
| Arduino Uno | The brain of the project; controls all sensors and motors. |
| L293D Motor Driver Module | Drives the four DC motors and controls direction and speed. |
| DC Gear Motors (x4) | Provide movement to the robot wheels. |
| Robot Wheels (x4) | Mounted on the gear motors for motion. |
| HC-SR04 Ultrasonic Sensor | Detects distance to obstacles by sending and receiving ultrasonic waves. |
| HC-05 Bluetooth Module | Enables communication between Arduino and a smartphone app. |
| Li-ion Batteries (x2) | Power source for the Arduino and motors. |
| Li-ion Battery Holder | Holds and connects the batteries securely. |
| Jumper Wires | Used for electrical connections between components. |
| Dot Board (or Breadboard) | Used for circuit assembly and wiring. |
| Switch | To power the robot ON/OFF easily. |

**Software Tools**
- Arduino IDE – for programming and uploading code to Arduino Uno  
- Bluetooth Controller App – used to control the robot manually from a smartphone (via Bluetooth)  
- Video Editing Tool – to edit and present the project video (e.g., Shotcut, CapCut, or DaVinci Resolve)

---

## Working Principle

### 1. Obstacle Avoidance Mode
- The ultrasonic sensor continuously measures the distance ahead.  
- If the distance to an obstacle is less than the set threshold (for example, 20 cm), the Arduino:  
  - Stops the motors.  
  - Turns the robot in a safe direction (left or right).  
  - Moves forward again once the path is clear.  

### 2. Bluetooth Control Mode
- The HC-05 Bluetooth module connects to a smartphone via a custom Android app.  
- Commands such as Forward, Backward, Left, Right, and Stop are sent from the app.  
- The Arduino receives these commands and drives the motors accordingly.

---

## Key Features
- Dual operating modes: Autonomous and Manual (Bluetooth)  
- Simple and efficient obstacle detection using ultrasonic waves  
- Reusable components — easy to modify or extend  
- Can be enhanced with voice control, camera, or line-following sensors  

---

## Circuit Overview
- Trigger Pin of the ultrasonic sensor → Arduino digital pin 9  
- Echo Pin → Arduino digital pin 8  
- Motor Driver (L293D) → Arduino pins 2, 3, 4, 5 for controlling motors  
- HC-05 Bluetooth Module:  
  - TX → Arduino RX (pin 0)  
  - RX → Arduino TX (pin 1)  
  - VCC → 5V  
  - GND → GND  
- Power Supply: 7.4V from two Li-ion batteries connected via the switch  

---

## Learning Outcomes
- Understanding the working of ultrasonic sensors and distance measurement  
- Interfacing Bluetooth modules with microcontrollers  
- Controlling DC motors using the L293D driver  
- Writing and uploading Arduino code for automation and communication  
- Gaining hands-on experience with embedded systems and robotics

---

## Project Demonstration

You can watch the working video of this project here:  
[Watch Project Video on Google Drive](https://drive.google.com/file/d/1XpzM8WvEN2O-NLphhWS1AU3YiFVYmo-s/view?usp=sharing)

---

## Author
 Mahnoor Yasir
 
---
