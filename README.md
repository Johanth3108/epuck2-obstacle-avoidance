# README

## Description
This repository contains code for controlling an e-puck robot to avoid obstacles using proximity sensors. The e-puck robot is equipped with infrared sensors to detect obstacles in its surroundings and maneuver accordingly to avoid collisions.

## Contents
- **main.c**: This file contains the main code for controlling the e-puck robot.
- **motors.h**: Header file containing motor control functions.
- **leds.h**: Header file containing functions to control LEDs on the e-puck.
- **spi_comm.h**: Header file for SPI communication.
- **sensors/proximity.h**: Header file for proximity sensor functions.
- **memory_protection.h**: Header file for memory protection.
- **ch.h**, **hal.h**: Header files for ChibiOS, a real-time operating system.
- **main.h**: Header file containing global declarations.
- **README.md**: This file.

## Requirements
- ChibiOS: This project is built on top of ChibiOS, a real-time operating system. Ensure that ChibiOS is properly installed and configured in your development environment.
- e-puck robot: The code is designed to run on an e-puck robot equipped with infrared proximity sensors.
- Compiler: Use a compatible C compiler to compile the code for the target platform.

## Usage
1. Clone the repository to your local machine:

```bash
git clone [https://github.com/Johanth3108/epuck2-obstacle-avoidance)]
```

2. Ensure all necessary dependencies are installed and configured, including ChibiOS.

3. Connect the e-puck robot to your development environment.

4. Compile the code using the appropriate compiler for your platform.

5. Upload the compiled binary to the e-puck robot.

6. Power on the e-puck robot and observe its behavior as it avoids obstacles using the proximity sensors.

## Functionality
The main functionality of the code is to control the movement of the e-puck robot based on readings from its infrared proximity sensors. The robot will:
- Move forward if no obstacles are detected.
- Turn left or right if obstacles are detected on either side.
- Stop if obstacles are detected in front of the robot.

## Customization
You can customize the behavior of the robot by adjusting parameters such as:
- Threshold values for obstacle detection (`THRESH`).
- Maximum acceleration of motors (`MAX_ACC`).
- Angular speed for rotation (`ANG_SPEED_DEG`).
- Duration of rotation for specific angles.

## Contributors
- Johanth PS (https://github.com/Johanth3108)
- Yuchi Wang ([https://github.com/prolouisw])
