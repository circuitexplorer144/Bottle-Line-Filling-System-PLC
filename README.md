# Bottle Line Filling System using PLC

## Project Overview

The Bottle Line Filling System is a PLC-based industrial automation project developed as part of Summer Internship training in Industrial Automation using PLC.

The project demonstrates the automation of a bottle filling process using ladder logic. The system is designed to control the movement of bottles through a filling station and perform the filling operation according to the programmed control sequence.

The project was developed and simulated using LogixPro 500, providing practical exposure to PLC programming, ladder logic, industrial control systems, timers, counters, and sequential automation.

---

## Objective

The main objectives of this project are:

- To understand the fundamentals of PLC-based industrial automation.
- To design a ladder logic program for an automated bottle filling process.
- To control the sequence of bottle movement and filling operations.
- To understand the use of PLC inputs and outputs in an automation system.
- To implement timers and counters for process control.
- To simulate and verify the PLC program using LogixPro 500.
- To gain practical experience in designing a sequential industrial automation system.

---

## Problem Statement

Manual bottle filling processes can require continuous human involvement and may lead to inconsistent filling operations, slower production, and increased chances of operational errors.

The objective of this project is to develop a PLC-based automated bottle filling system that can control the bottle movement and filling process according to a predefined sequence.

The PLC monitors the input conditions and activates the required outputs using ladder logic to automate the complete process.

---

## Features

- PLC-based automated bottle filling process.
- Ladder logic-based control system.
- Sequential control of the filling operation.
- Automatic control of the bottle movement process.
- Timer-based control for process operations.
- Counter-based bottle counting.
- Simulation using LogixPro 500.
- Easy-to-understand industrial control logic.
- Demonstrates practical PLC programming concepts.
- Suitable for basic industrial automation applications.

---

## Software and Tools

### Software Used

- LogixPro 500 Simulator

### Concepts Used

- Programmable Logic Controller (PLC)
- Ladder Logic Programming
- Digital Inputs and Outputs
- Timers
- Counters
- Sequential Control
- Industrial Automation
- Motor/Conveyor Control
- Sensor-Based Control

---

## PLC Details

The project is based on PLC programming concepts using ladder logic.

The PLC acts as the main controller of the bottle filling system. It receives signals from input devices such as sensors and push buttons and processes these signals according to the ladder logic program.

Based on the programmed conditions, the PLC controls the required output devices such as the conveyor motor and filling mechanism.

### PLC Functions in the Project

- Monitoring input conditions.
- Detecting bottle positions.
- Controlling the conveyor operation.
- Controlling the filling operation.
- Maintaining the required filling time.
- Counting bottles.
- Executing the programmed sequence.
- Providing automatic process control.

---

## Inputs and Outputs

The system consists of digital input and output devices used to control the bottle filling process.

### Inputs

Typical input devices used in the system include:

| Input | Function |
|---|---|
| Start Push Button | Starts the automated process |
| Stop Push Button | Stops the process |
| Bottle Detection Sensor | Detects the presence/position of a bottle |
| Other Sensors | Provides process-related input conditions |

### Outputs

Typical output devices include:

| Output | Function |
|---|---|
| Conveyor Motor | Moves bottles through the production line |
| Filling Mechanism | Performs the bottle filling operation |
| Indicator/Status Output | Indicates the operating condition |
| Other Control Outputs | Controls process-related devices |

> Note: The exact PLC addresses and I/O configuration are based on the ladder logic developed for the project.

---

## Working Principle

The Bottle Line Filling System works according to a predefined PLC control sequence.

1. The system is started using the Start push button.
2. The PLC checks the required input conditions.
3. The conveyor system is activated to move the bottle toward the filling station.
4. The bottle detection sensor detects the bottle at the required position.
5. The PLC stops or controls the conveyor according to the programmed sequence.
6. The filling mechanism is activated.
7. A timer controls the required filling duration.
8. After completion of the filling operation, the filling mechanism is deactivated.
9. The conveyor resumes operation to move the filled bottle forward.
10. The counter keeps track of the bottles processed by the system.
11. The sequence continues automatically for subsequent bottles.
12. The Stop input can be used to stop the system.

The complete process is controlled automatically by the PLC using ladder logic.

---

## Ladder Logic Explanation

The ladder logic program is designed using standard PLC programming concepts.

### 1. Start/Stop Control

The Start push button is used to initiate the system operation.

The Stop push button provides a method to stop the automated process.

The start/stop logic ensures that the system operates only when the required control conditions are satisfied.

### 2. Bottle Detection

A sensor is used to detect the presence of a bottle at the required location.

When the sensor detects a bottle, the PLC receives the corresponding input signal.

This signal is used by the ladder logic to control the next stage of the process.

### 3. Conveyor Control

The conveyor output is controlled by the PLC.

When the required conditions are satisfied, the conveyor motor is energized to move the bottles toward the filling station.

When a bottle reaches the required filling position, the conveyor operation is controlled according to the programmed sequence.

### 4. Filling Control

After the bottle reaches the filling station, the PLC activates the filling mechanism.

The filling operation remains active for the programmed duration.

A timer is used to control the filling period.

### 5. Timer Control

The timer provides a controlled time delay for the filling operation.

After the preset time is completed, the timer's done condition is used by the ladder logic to deactivate the filling output and continue the process.

### 6. Bottle Counting

A counter can be used to maintain the number of bottles processed by the system.

Whenever a complete bottle filling cycle is detected, the counter increments its value.

This provides a simple method of monitoring production quantity.

### 7. Sequence Control

The different ladder logic conditions work together to create a sequential control system.

The PLC continuously scans the inputs, executes the ladder logic, and updates the outputs according to the current process conditions.

---

## Control Sequence

The basic control sequence of the system can be represented as:

```text
START
   ↓
Check System Conditions
   ↓
Conveyor ON
   ↓
Bottle Detection
   ↓
Bottle Reaches Filling Station
   ↓
Conveyor Control
   ↓
Filling Mechanism ON
   ↓
Timer Starts
   ↓
Filling Time Completed
   ↓
Filling Mechanism OFF
   ↓
Conveyor ON
   ↓
Bottle Moves Forward
   ↓
Bottle Counter Increment
   ↓
Next Bottle
   ↓
Repeat Process
```
```

````
## Timer and Counter Usage

### Timer

A timer is used to control the duration of the bottle filling operation.

The timer ensures that the filling mechanism remains active for the required period. Once the preset time is completed, the filling operation is stopped and the process continues to the next stage.

General operation:

```text
Bottle Detected
      ↓
Filling Mechanism ON
      ↓
Timer Starts
      ↓
Preset Time Completed
      ↓
Filling Mechanism OFF
      ↓
Process Continues
````

### Counter

A counter is used to keep track of the number of bottles processed by the system.

After a bottle completes the required filling cycle, the counter can be incremented to maintain the production count.

General operation:

```
```

```
Bottle Filling Completed
        ↓
Counter Trigger
        ↓
Counter Value Increases
        ↓
Production Count Updated
```

---

## LogixPro 500 Simulation

The Bottle Line Filling System was simulated using the LogixPro 500 PLC simulator.

The simulation was used to test and verify the ladder logic before considering practical implementation.

The simulation helped in understanding the interaction between PLC inputs, outputs, timers, counters, and the bottle filling sequence.

### Simulation Objectives

-  To verify the ladder logic operation. 
-  To test the bottle detection sequence. 
-  To check conveyor control. 
-  To verify the filling operation. 
-  To test timer functionality. 
-  To verify bottle counting. 
-  To identify and correct logic errors. 
-  To observe the complete automated sequence. 

### Simulation Result

The LogixPro 500 simulation demonstrated the programmed bottle filling sequence and provided practical experience in PLC-based industrial automation.

---

## Project Workflow

The project was developed using the following workflow:

```
```

```
Industrial Automation Concept
          ↓
Process Analysis
          ↓
Identify Inputs and Outputs
          ↓
Develop Control Sequence
          ↓
Design Ladder Logic
          ↓
Implement PLC Program
          ↓
Simulate in LogixPro 500
          ↓
Test Inputs and Outputs
          ↓
Verify System Operation
```

---

## Results

The Bottle Line Filling System successfully demonstrates the basic automation of a bottle filling process using PLC ladder logic.

The project demonstrates:

-  PLC-based process control. 
-  Sequential automation. 
-  Sensor-based operation. 
-  Conveyor control. 
-  Timer-based filling control. 
-  Counter-based production monitoring. 
-  Ladder logic programming. 
-  PLC simulation and testing. 

The LogixPro 500 simulation helped verify the programmed control sequence and provided practical experience with industrial automation concepts.

---

## Learning Outcomes

Through this project, I gained practical knowledge of:

-  PLC programming fundamentals. 
-  Ladder logic design and implementation. 
-  Digital input and output control. 
-  Industrial automation concepts. 
-  Sensor-based process control. 
-  Conveyor-based automation. 
-  Timer and counter instructions. 
-  Sequential control logic. 
-  PLC troubleshooting and testing. 
-  LogixPro 500 simulation. 
-  Converting a real-world industrial process into PLC control logic. 

---

## Future Improvements

The system can be further improved by implementing:

-  Automatic bottle level detection. 
-  Adjustable filling volume. 
-  HMI-based monitoring and control. 
-  Real-time production monitoring. 
-  Emergency stop and safety interlocks. 
-  Fault detection and alarm systems. 
-  Improved sensor-based bottle detection. 
-  SCADA system integration. 
-  Production data logging. 
-  IoT-based remote monitoring. 

---

## Project Applications

The concepts demonstrated in this project can be applied to industrial processes such as:

-  Bottle filling plants. 
-  Beverage industries. 
-  Packaging industries. 
-  Manufacturing automation. 
-  Conveyor-based production lines. 
-  Automated material handling systems. 
-  Industrial process control. 

---

## Project Resources

### Ladder Diagram

The complete ladder diagram used for the Bottle Line Filling System:

[View Ladder Diagram](Ladder_Diagram/Bottle_Line_Filling_Ladder_Diagram.png)

### LogixPro 500 Simulation

The LogixPro 500 simulation screenshot:

[View Simulation](Simulation/Bottle_Line_Filling_LogixPro_Simulation.png)

### Training Certificate

The Industrial Automation / PLC training certificate:

[View Training Certificate](Certificate/Industrial_Automation_PLC_Training_Certificate.pdf)


## Training

This project was developed as part of Summer Internship training in Industrial Automation using PLC.

The training provided practical exposure to:

-  PLC architecture 
-  Input/Output modules 
-  Process scanning 
-  Ladder logic 
-  PLC programming 
-  Timers and counters 
-  Industrial control logic 
-  LogixPro 500 simulation 
-  Automation system design 

---

## Technologies and Skills

**PLC:** Programmable Logic Controller

**Programming:** Ladder Logic

**Simulation:** LogixPro 500

**Domain:** Industrial Automation

**Concepts:** PLC Programming, Digital I/O, Timers, Counters, Sequential Control, Conveyor Automation

---

## Author

**Anshu Chauhan**

B.Tech – Electronics and Communication Engineering

Interested in Embedded Systems, Hardware, Electronics, and Industrial Automation.

### Areas of Interest

-  Embedded Systems 
-  Electronics 
-  Hardware Design 
-  Industrial Automation 
-  PLC Programming 
-  Microcontrollers 
-  IoT Systems ...i am going paste this same in  raedmefile
