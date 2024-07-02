# Edge-Avoider-Robot
Edge-Avoiding Robot Controller
This repository contains code to control an edge-avoiding robot using an ESP32 microcontroller. The robot uses two sensors to detect the edges of a surface and adjusts its movement to avoid falling off.

Table of Contents
Overview
Hardware Requirements
Pin Configuration
Installation
Usage

Overview
This project demonstrates how to control an edge-avoiding robot using an ESP32 microcontroller. The robot uses two sensors to detect edges of a surface and changes its direction to avoid falling off. The code enables the robot to move forward, backward, and turn left or right based on the sensor input.

Hardware Requirements
ESP32 Wroom 32D Development Board
Motor Driver (e.g., L298N)
Two DC Motors
Two edge detection sensors (e.g., IR sensors or cliff sensors)
Power supply for the motors
Connecting wires
Pin Configuration
ESP32 Pin	Description
17-	Motor Left (ML1)
5-	Motor Left (ML2)
4-	Motor Right (MR1)
16	-Motor Right (MR2)
19-	Left Sensor
18-	Right Sensor
Installation
Clone this repository:

sh
Copy code
git clone https://github.com/yourusername/edge-avoiding-robot.git
Open the project in the Arduino IDE or your preferred development environment.

Connect your ESP32 to your computer.

Select the appropriate board and port in the Arduino IDE.

Upload the code to your ESP32.

Usage
Connect the motors and sensors to the ESP32 according to the pin configuration table.

Power up the ESP32 and the motor driver.

Open the Serial Monitor in the Arduino IDE to view the sensor values and movement directions.

Place the robot on a surface where it can detect edges.

The robot will move based on the sensor input:

Move forward if both sensors do not detect an edge.
Move backward and then turn left if both sensors detect an edge.
Turn left if only the left sensor detects an edge.
Turn right if only the right sensor detects an edge.










