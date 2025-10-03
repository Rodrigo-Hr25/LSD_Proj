# Air Conditioning System Simulator

## Overview

This repository showcases a comprehensive VHDL project developed at the **University of Aveiro**. The project simulates an air conditioning system with an embedded remote control, demonstrating proficiency in digital system design, hardware description languages, and FPGA-based simulation.

## Project Context

The project was undertaken as part of the *Digital Systems Logic* course at the University of Aveiro. The primary objective was to design and simulate the logic of an air conditioning system, integrating both the control unit and the remote control functionalities using VHDL. This endeavor aimed to replicate the behavior of a real-world air conditioning unit within a simulated environment.

## System Architecture

The system is structured into several key modules:

* **Main Controller (Finite State Machine - FSM):** Manages the overall operation, including power states, mode selection, and temperature adjustments.
* **Temperature Control Module:** Handles the increase and decrease of the target temperature, simulating user input and system response.
* **Mode Selector:** Allows switching between different operating modes such as cooling, heating, and ventilation.
* **Remote Control Logic:** Embeds the functionality of a remote control, enabling user interaction through simulated inputs.
* **Display/Output Module:** Simulates the system's feedback, such as displaying the current temperature and active mode.

## Key Components in the Repository

* **`ProjetoFinal.vhd`**: The top-level module that integrates all other components into a cohesive system.
* **`FSM.vhd` / `FSM_Tb.vhd`**: Defines the finite state machine and includes a testbench for simulation purposes.
* **`DisplayUnit.vhd` / `DisplayUnitTemp.vhd`**: Handles 7-segment display control, converting BCD values into display signals.
* **`Bin2BCD.vhd`, `Bin9Bits2BCD.vhd`, `Bin7SegDecoderEn.vhd`**: Conversion modules that allow numerical values to be correctly represented on the displays.
* **`Relogio.vhd` / `RelogioControler.vhd` / `count24.vhd` / `count60.vhd`**: Counters and timing modules used for temporal operations within the system.
* **`DebounceUnit.vhd`**: Ensures reliable button input by removing signal noise from physical or simulated presses.
* **`Ram_1P_32x2.vhd` / `Ram_1P_32x2_Tb.vhd`**: Implements a small single-port RAM for storing system parameters or states.
* **`BlinkPulseGenerator.vhd`, `BlinkOperation.vhd`, `pulse_gen.vhd`**: Modules responsible for generating pulse and blink signals for LEDs or timing indications.
* **`simulador_ambiente.vhd`**: Simulates external inputs such as user commands and environmental changes to test system behavior.

## Implemented Features

* **Power Control:** Enables turning the system on and off.
* **Temperature Adjustment:** Allows setting and modifying the desired temperature.
* **Operating Modes:** Supports selection between cooling, heating, and ventilation modes.
* **Integrated Remote Control:** Incorporates remote control logic within the system, simulating real-world usage scenarios.

## Technical Skills Demonstrated

* **VHDL Programming:** Utilization of VHDL for designing and simulating digital systems.
* **Finite State Machine Design:** Implementation of FSMs to manage system states and transitions.
* **Modular System Design:** Creation of reusable and testable modules for system components.
* **FPGA Simulation:** Testing and validation of the design using FPGA simulation tools.

## Educational Context

This project was developed as part of the coursework at the **University of Aveiro**, reflecting both theoretical knowledge and practical skills in digital system design, hardware description, and embedded system simulation.
