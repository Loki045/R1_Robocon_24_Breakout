# R1_Robocon_24_Breakout
Breakout and control interface PCB designed for Robocon 2024 R1 robot, supporting Arduino Mega + Host Shield stacking, motor control interfaces, and regulated power distribution from external supply modules.

# Robocon 2024 – R1 Control Breakout PCB

This repository contains the hardware design files for the **R1 Control Breakout PCB** used in the Robocon 2024 robot.

The board was designed to serve as a **stackable control and interface breakout**, enabling easy connection of motors, actuators, and control modules using an **Arduino Mega + Host Shield** stack.

---

## 📌 Robot Task Overview

In Robocon 2024, **Robot 1 (R1)** performed the following operations:

- Navigated across Area 1
- Picked up seedlings
- Placed up to **12 seedlings** into assigned circular positions
- Moved to Area 2
- Threw balls in alternating sequence:
  - Team-colored ball (Red/Blue)
  - Violet ball
  - Repeat sequence
- Threw balls toward Area 3 based on number of successfully placed seedlings

This PCB supported the control and actuator interfacing required to perform these tasks.

---

## ⚙️ Board Overview

The R1 PCB was designed as a **centralized control breakout board**, allowing:

- Direct mounting of **Arduino Mega**
- Stacking of **USB Host Shield**
- Organized connection of motors and actuators
- Easy access to multiple communication pins
- Distribution of regulated voltages received from an **external power distribution board**

This modular approach simplified robot wiring and improved system maintainability.

---

## 🔧 Key Features

- Arduino Mega compatible stacking layout
- USB Host Shield support (for controller interface)
- 4 PWM motor connectors for locomotion control
- Servo motor connectors
- Stepper motor connectors
- BLDC motor interface connectors
- Kill switch interface
- External indicating lamp connectors
- Extra UART headers
- Additional GPIO expansion pins
- LED power/status indicators
- Decoupling capacitors for stable operation

---

## 🔌 Power Interface

Regulated voltages were supplied from an **external power distribution board**.

### Input Power (via Screw Terminals):

- 12V Input
- 7.4V Input
- 5V Input

### On-board Power Headers:

- 7.4V Output Headers
- 5V Output Headers
- GND Headers

These headers enabled clean routing of regulated voltages to connected modules.

---

## 🎮 Motor & Actuator Interfaces

### Locomotion Control:

- 4 PWM output connectors for Cytron Smart Drive Mdds30 Dual 30A motor driver

### Actuator Support:

- Multiple Servo connectors
- Stepper motor connectors
- BLDC motor interface connectors

These supported the mechanisms required for seedling placement and ball throwing operations.

---

## 🧩 Additional Interfaces

- Kill Switch Connector
- External Indicator Lamp Connectors
- Extra UART Communication Headers
- General-Purpose GPIO Expansion Pins
- LED Indicators for Power/Status Monitoring

---

## 🧰 Hardware Stack

Designed to support:

- Arduino Mega 2560 (Main Controller)
- USB Host Shield
- Redgear Controller (via Host Shield)

This stack allowed wireless/manual control of the robot.

---

## 📂 Repository Contents

R1_PCB_2024-25_VRC/

    ├── PCB Layout File
    ├── Project File
    ├── Schematic File 
Images/

    ├── Top Layer View  
    ├── Bottom Layer View  
    ├── 3D View  
      
.gitignore

README.md

---

## 🛠 Tools Used

- KiCad — Schematic and PCB Design
- Arduino IDE — Firmware Development


---

## 🎯 Application

This PCB was used in the **Robocon 2024 R1 robot**, providing structured connectivity for locomotion motors, actuators, and control interfaces required for seedling placement and ball-throwing operations.

---

## 👨‍💻 Contribution

Developed as part of the Robocon 2024 electronics system, contributing to hardware layout planning, connector design, and system-level integration for robot subsystems.

---

## 📸 PCB Images

- Schematic
  
  <img width="1311" height="877" alt="image" src="https://github.com/user-attachments/assets/b0d87dcd-6ec5-4bd7-aa51-0989248200cd" />
 
- F.Cu Layer View
  
   <img width="646" height="497" alt="image" src="https://github.com/user-attachments/assets/5ed7b7ef-9888-450e-9e2c-6fce44024c55" />
   
- B.Cu Layer View
  
  <img width="644" height="494" alt="image" src="https://github.com/user-attachments/assets/9b0e93bd-385a-4c5f-91eb-264c03f14afb" />

- 3D View
  
  <img width="1723" height="952" alt="R1_PCB_2024-25_VRC" src="https://github.com/user-attachments/assets/420a5a93-928e-4e54-b5dd-e95c95cf61c0" />

---

## 📎 Design Intent

This board was designed to reduce wiring complexity, improve modularity, and enable rapid maintenance during robot testing and competition.
