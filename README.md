# The Pink Pony Picker Pucker - 3rd Place

This code is for an autonomous robot that competed at MICS in 2026. Took 3rd place.

## Overview

This robot was designed to run on a board with 3 other robots and find the pucks assigned at the start of the match. You also could not purposefully run into the other team's robot. You were randomly assigned one of four colors at the beginning of each match. I worked on this mostly solo but with assistance from other classmates. 

## Hardware

- Raspberry Pi
- Motors with a motor driver
- Omni wheels
- Breadboard
- Camera sensor
- 3D-printed body
- 
## Software

- Language: Python 3
- Libraries: RPi.GPIO (motor control), Tkinter (GUI)

## How It Works

The motor shield's GPIO pins control each wheel's speed and direction, using PWM to set speed. Movement in each direction comes from combining the four wheel speeds using the standard mecanum formula:

- Front-left and rear-right = forward + strafe
- Front-right and rear-left = forward − strafe

For example, driving the front-left and rear-right wheels forward while the other two go backward makes the robot strafe right.

## Running the Code
1. Install dependencies on the Raspberry Pi:

## What I Learned

I learned that more complexity doesn't always mean better. This competition was very complex, and I relied on my resources, like my peers, professors, and AI, to help guide me. The hardest part for me was avoiding other robots. Without the avoidance code, every component worked, but once it was active, there was too much happening at once. I learned a lot and worked with hardware I had never used before, like a breadboard and using a camera as a sensor.
