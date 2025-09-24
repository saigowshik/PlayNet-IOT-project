PlayNet – IoT Gaming System
Overview
PlayNet is an IoT-based interactive gaming system that merges physical ball play and virtual maze navigation into one project.
It uses ESP32, Arduino UNO R4, sensors, and actuators to provide a dual-game experience, all controlled via smartphone in Access Point (AP) mode.
Project Modules
1. PlayNet – Motorized Tube Game
ESP32 (AP Mode): Hosts a webpage for motor speed control (Levels 1–10).
HW-039 H-Bridge + 775 DC Motor: Spins a rotating tube.
UNO R4 + Ultrasonic Sensor: Detects when a ball is thrown into the tube.
Buzzer: Gives feedback when a ball is successfully detected.
2. Maze Game – Virtual Challenge
ESP32 (AP Mode): Connects to phone and processes sensor input.
ADXL345 Gyroscope: Provides tilt control for navigating the maze.
0.95" OLED Display: Shows maze path and ball movement from start to finish.
Displays “You Win” when the maze is completed.
Features
Smartphone connection in AP mode (no internet required).
Web-based interface to control motor speed and interact with the game.
Dual Gameplay: Physical ball game + virtual maze challenge.
Real-time feedback: OLED messages, buzzer alerts, and motor control.
Scalable Design: Can be extended with scoring, leaderboards, or cloud storage.
Components
ESP32 (x2)
Arduino UNO R4 (x1)
775 DC Motor (x1)
HW-039 H-Bridge Motor Driver (x1)
Ultrasonic Sensor HC-SR04 (x1)
ADXL345 Gyroscope (x1)
0.95" OLED Display (x1)
Piezo Buzzer (x1)
Breadboard / PCB, Jumper Wires, Resistors, Capacitors
Power Supply (12V for motor, 5V for logic)
Smartphone (for AP mode connection)
How It Works
Connect your smartphone to the ESP32’s Wi-Fi AP.
Open the hosted webpage:
Select motor speed (1–10 levels).
Start the PlayNet rotating tube game.
When the ball enters the tube:
Ultrasonic sensor detects it.
Buzzer sounds for feedback.
Switch to the Maze Game module:
Tilt the ADXL345 to move the ball on OLED display.
Reach the goal to win!
Applications
Educational tool for IoT + Embedded Systems.
Fun and portable arcade-style game.
Enhances hand–eye coordination and logical thinking.
Prototype for future IoT arcade gaming platforms.
Conclusion
PlayNet demonstrates how IoT can merge physical and digital games into a unified experience.
It highlights creativity in combining sensors, microcontrollers, and real-time feedback systems, making it a fun, educational, and scalable project.
