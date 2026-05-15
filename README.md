# 6-DOF Educational Robotic Arm

## Overview
The goal of this project is to develop a cost-effective robotic arm system designed as an educational platform for student learning and hands-on training. The robotic arm was developed based on design references from the AR4 robotic arm platform and an educational robotic arm model developed by Huynh Khanh Toan from Ho Chi Minh City University of Technology and Education (HCMUTE).
<p align="center">
  <img src="https://github.com/user-attachments/assets/c8fe3097-9de5-49e2-b3c1-6bde086d1aca" height="350"/>
  <img src="https://github.com/user-attachments/assets/551e08f7-9203-445f-a131-785177ff184e" height="350"/>
</p>



## Technical Scope
- Designed a 6-degree-of-freedom robotic arm structure using SolidWorks.
- Developed an STM32-based servo controller with I2C communication.
- Integrated six servo motors with ESP32 as the primary MCU.
- Implemented Forward/Inverse Kinematics with interpolation algorithms.
- Designed the electrical control panel in AutoCAD and developed the controller circuitry in Altium Designer.
- Developed an Android application with custom UI/UX for robotic arm control via TCP/IP communication.

## System Architecture
The robotic arm system architecture consists of:
- ESP32 as the primary communication and high-level control MCU
- STM32-based servo control modules for lower-load joints (J1, J5, and J6)
- Ezi-Plus R servo systems for joints J2, J3, and J4 due to higher torque and load requirements
- Android application for wireless robot operation via TCP/IP communication
- Custom-designed controller circuitry and electrical control panel for power distribution

## Software Features
- Forward/Inverse Kinematics calculation
- Motion interpolation for smooth trajectory control
- Real-time servo position control
- TCP/IP communication between Android application and robotic arm

## Design Iterations
### Version 1
- Initial prototype focused on basic robotic arm movement and servo integration
- Implemented basic angle control for all 6 robotic joints
- Tested STM32-based servo communication package
- Evaluated initial mechanical structure and motion performance on each joint
### Version 2
- Redesigned the linkage structure of joint 4, 5 and 6 to improve rigidity and stability
- Implemented Forward and Inverse Kinematics with interpolation algorithms
- Updated the PCB and electrical control panel design for improved system integration
- Implemented synchronized motion control for all 6 robotic joints
- Integrated a pneumatic gripper for handling objects weighing under 1 kg
- Integrated ESP32 wireless communication system
- Developed Android-based robotic arm control application

<img width="1185" height="664" alt="image" src="https://github.com/user-attachments/assets/73370056-deca-4205-a492-7138e971b4eb" />


## Full Demonstration Video
[Watch on YouTube](https://youtu.be/26i8T7e-IkA)

## Future Improvements
- Closed-loop feedback control
- Vision-based object detection
- Trajectory planning optimization
- ROS integration
- Industrial-grade actuator upgrade
- End-effector expansion support

