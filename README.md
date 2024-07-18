# Graduation_Project_ADAS

## Overview

This project is developed by a team of 8 students from Al-Azhar University. The goal was to implement an autonomous vehicle system featuring Lane Keeping Assist (LKA), Adaptive Cruise Control (ACC), Blind Spot Warning (BSW), Lane Departure Warning (LDW), and Traffic Sign Recognition (TSR) using AI.

## System Architecture

The system consists of three main boards:

1. **STM32F103**: 
   - **Role**: Master ECU
   - **Responsibilities**: Runs the main logic of the system, deals with actuators like DC and servo motors.
   - **Operating System**: FreeRTOS
   - **Communication**: Connected to the Sensors HUB (STM32F401) via SPI and to the Raspberry Pi 4 via UART.

2. **STM32F401**:
   - **Role**: Sensors HUB
   - **Responsibilities**: Manages sensors such as ultrasonic sensors and motor encoders.
   - **Operating System**: FreeRTOS

3. **Raspberry Pi 4**:
   - **Role**: AI Processing Unit
   - **Responsibilities**: Runs AI models for lane detection and sign detection, handles camera input, and runs the car control application.
   - **Communication**: Connected to the Master ECU via UART.

## Features

- **Lane Keeping Assist (LKA)**: Keeps the vehicle within its lane.
- **Adaptive Cruise Control (ACC)**: Automatically adjusts the vehicle speed to maintain a safe distance from vehicles ahead.
- **Blind Spot Warning (BSW)**: Alerts the driver to vehicles in the blind spots.
- **Lane Departure Warning (LDW)**: Warns the driver when the vehicle begins to move out of its lane.
- **Traffic Sign Recognition (TSR)**: Detects and recognizes traffic signs.

## Hardware Implementation

The project was successfully implemented in hardware. You can view the system in action through this [link](https://drive.google.com/drive/folders/1Reht7Lhxi9n5DfqujkTGu-U8IwrOOwM4).

- [Your Name]

## University

- **Al-Azhar University**
