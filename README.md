# MicroMouse Project: Sensing and Power Subsystems

Welcome to the MicroMouse Project repository! The problem this entire project deals with is to design, build, and test a fully-functioning MicroMouse robot. Akin to the mice in the famous Kerplunk Experiments, a MicroMouse robot should be able to solve a maze using the shortest and fastest route possible. This README provides an overview of the project and subsystem descriptions.

## Project Overview

The goal of this project is to build key subsystems for a simplified MicroMouse, a maze-solving robot. These will be designed, manufactureed, and tested during the course of a semester.

## Subsystems

### 1. Power Subsystem (more info [here](Power Subsystem))
- **Purpose:** Provide power to the entire system.
- **Key Functions:**
  - Operate two motors (each drawing up to 200mA).
  - Charge the battery from a 5V input.
  - Provide battery voltage information to the processor.
  - Include an ON/OFF switch with specific power draw requirements.
- **Connections:**
  - JST PH 2mm pin pitch connector for the battery.
  - 2x8 (2.54mm pin pitch) pin header for interfacing with the motherboard.<br />
  ![image](https://github.com/ZuhayrHalday/EEE3088F-Micromouse-Project/blob/main/Power%20Subsystem/PCB%20images/3D%20view.png)<br />

### 2. Sensing Subsystem (more info [here](Sensing Subsystem))
- **Purpose:** Detect obstacles in the robot's path.
- **Key Functions:**
  - Detect obstacles in front and on the sides of the robot.
  - Use power-saving features when not in operation.
  - Provide reliable detection data to the processor.
  - Interface with processor LEDs to indicate detected obstacles.
- **Connections:**
  - 2x14 (2.54mm pin pitch) pin header for interfacing with the motherboard.<br />
  ![image](https://github.com/ZuhayrHalday/EEE3088F-Micromouse-Project/blob/main/Sensing%20Subsystem/PCB%20Schematics%20and%20Gerbers/3DPCB.png)<br />

### 3. The Motherboard
The Motherboard houses all subsystems and addresses the movement and ‘brain’ aspects of the project. The
wheels and motors of the MicroMouse are attached to the Motherboard PCB, which also mounts an STM32L476
microcontroller to manage input and output logic. Pin headers are provided for interfacing with other subsystems.
