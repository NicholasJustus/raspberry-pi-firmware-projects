# Raspberry Pi Firmware Projects

## Overview
In this course, I worked on building Python programs that interact with real hardware using a Raspberry Pi. The goal was to understand how software can control physical components like LEDs, buttons, sensors, and an LCD display.

The two main projects I included here are a smart thermostat system and a LED state machine. Both projects helped me understand how to structure logic for hardware control and how to debug both code and circuits at the same time.

## Project 1: Smart Thermostat
This project simulates a basic thermostat system using a temperature sensor, buttons, LEDs, and a 16x2 LCD display.

The thermostat has three states: off, heat, and cool. A button cycles through these states. The system compares the current temperature to a set temperature and reacts based on that.

- In heat mode, the red LED fades if the temperature is below the setpoint, and stays solid if it reaches it  
- In cool mode, the blue LED fades if the temperature is above the setpoint, and stays solid when it cools down  
- The LCD displays the current temperature, system state, and setpoint  
- The system also sends updates over serial communication every 30 seconds  

One thing that made this project more challenging was getting everything working together at the same time. I had to make sure the sensor readings, button inputs, LED behavior, and display updates all stayed in sync. I also ran into issues where I thought something was wrong with my code, but it turned out to be wiring problems, so I had to debug both hardware and software together.
<img width="490" height="487" alt="image" src="https://github.com/user-attachments/assets/36dc8787-1d88-4435-8e34-da83343e47be" />
<img width="487" height="439" alt="image" src="https://github.com/user-attachments/assets/f311ab21-c7e2-4371-aa0f-6c21506e27e1" />
<img width="478" height="375" alt="image" src="https://github.com/user-attachments/assets/a50b0e99-ef2a-4eb8-a5f8-808b3cdfcc75" />


## Project 2: LED State Machine
This project is a simpler example that helped me understand how state machines work before building the thermostat.

A button press cycles between different LED states:
- Off
- Red LED fading
- Blue LED fading

This project helped me understand how to organize logic using states instead of writing everything in one block of code. Once I understood this, it made the thermostat project much easier to build.

## What I Did Well
I think I did a good job connecting software logic to real hardware. I was able to get multiple components working together and responding correctly to inputs.

I also got more comfortable using state machines to control behavior, which made my code more organized and easier to follow.

## Where I Can Improve
One area I can improve is planning out my logic before I start coding. There were times where I had to go back and fix things because I didn’t fully think through how everything should work together.

I also want to get better at debugging hardware faster. Sometimes I spent too long figuring out whether the issue was the code or the wiring.

## Tools and Resources
- Python (main programming language)
- Raspberry Pi GPIO libraries (gpiozero, RPi.GPIO)
- statemachine library
- Serial communication
- Course materials and documentation

## Transferable Skills
This project helped me build skills that apply to other areas like embedded systems and firmware development. This includes working with hardware, using state machines, debugging issues, and thinking about how systems behave over time.

## Code Quality
I tried to keep my code readable by organizing it into classes and separating different responsibilities. The state machine approach also helped keep the logic clean and easier to maintain.

If I were to improve this further, I would add more comments and clean up some sections to make them easier to understand at a glance.m
