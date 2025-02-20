---
title: "UAV Forge"
excerpt_separator: "<!--more-->"
categories:
  - Blog
tags:
  - UAV Forge
---

# [UAV Forge at UCI](https://sites.uci.edu/uavforgeuci/)

While completing my B.S. in Mechanical Engineering at UC Irvine, I was a member of UAV Forge at UCI from 2019-2022 working on various subsystems. This project was dedicated to the development of a UAV and UGV for the [sUAS competition](https://suas-competition.org/) for the respective years.

## The specific platforms I worked in the design, fabrication, and testing of include:
* 4ft wingspan hexacopter
* 2ft wingspan quadcopter (autonomous testing)
* 1x2ft rovers
* 8ft wingspan fixed-wing test-bed
* 4ft wingspan pusher-config test-bed

##Responsibilities
### Hexacopter
+ Avionics
  * Developed python script to detect Wind Speed and Direction using Differential Pressure Sensors
+ Structures
  * Wrote MATLAB script to model dodeled stress on multi-rotor composite carbon fiber arms from rotor thrust using FEA
  * Validated software against ANSYS and Solidworks Simulations within 5% error
+ Dynamics and Propulsions
  * Optimized component specifications for flight-time and Thrust-to-Weight (TWR) Ratio using [thrust simulation software](https://www.ecalc.ch/)
  * Devloped custom electronic drive simulation tool in python to model flight performance of multi-rotors considering
    - TWR
    - Flight-Time
    - Propeller Size
    - Motor Performance
    - Atmospheric Conditions
+ Flight Testing
  * Leveraged PID control laws to tune motors using ArduPilot
  * Developed Way-point navigation tests in ArduPilot and evaluated accuracy using telemetry data and visual testing
### Fixed-Wings
+ Fabrication
  * Created fabrication files for various geometry using 3D Printers and Laser Cutters to enable modular design and rapid prototyping
  * Developed assembly documentation to reduce construction time from 1 week to 4 hours leveraging modular brackets allowing for wing, tail, and body geometry to be "hot-swappable"
+ Aerodynamics
  * Simulated air-foil and wing performance in [xflr5](http://www.xflr5.tech/xflr5.htm) and [xfoil](https://web.mit.edu/drela/Public/web/xfoil/)
  * Simulated Lift an Drag generation in MATLAB to determine optimum flight speed at max altitude for minimum drag
+ Propulsion
  * Optimzed motor, propeller, and esc, component specifications to maximize thrust and minimize battery consumption for a minimum endurance of 20 minutes
  * Conducted Static Tests to validate battery consumption models
### Rovers
+ Package Drop
  * Designed parachutes for dropping UGV's in flight from 100ft altitude without damaging system
  * Optimized UGV design using modular frame components to allow for motor and wheel swaps in under 3 minutes
  * Modeled force of impact on UGV structure using Solidworks simulation packages to verify design
  * Modeled forces on winch spool to verify material choice and design would not yield during descent
+ Navigation
  * Developed path planning algorithms A*, R*, and verified simulation performance against Dijkstra's Algorithm
  * Tested A* and R* against trained genetic algorithm and built in Ardu-Pilot waypoint navigation

### Hexacopter
<embed src="http://example.com/the.pdf" width="500" height="375" 
 type="application/pdf">
