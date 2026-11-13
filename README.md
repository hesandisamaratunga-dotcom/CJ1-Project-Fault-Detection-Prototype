# Fault Detection Prototype: Multi-Node Sensor Monitoring & Protection

Elective Project 1 (CJ1), B.Sc. Information Engineering, HAW Hamburg

Supervisor: Prof.Dr. Frerk Haase
Team: Hesandi Samarathunga, Rithika Ganeshan, Pansiluni Samarakoon
Start date: September 2026

# Project description

We build a small, safe, low-voltage radial test network and use it to study fault detection.

The network has a source branch, two nodes (node 1, node 2) and a fault branch.
Three INA219 sensors measure voltage and current at the source and at each node.
An ESP32 monitor reads the sensors and runs a local NORMAL / WARNING / TRIP protection state machine.
Readings and state changes go over serial to a laptop, into a database, and onto a live dashboard.
A 4-channel oscilloscope records the same events. We use it to measure sensor accuracy and fault-detection latency.

# Why this project:

Power grids need monitoring that detects short circuits, overloads and voltage sags early.
The project combines circuit hardware, embedded sensing and software-based data analysis.
