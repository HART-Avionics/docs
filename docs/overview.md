Project Overview
==================

## Goals
----------
The HART team's ultimate goal is to launch a rocket up to 150,000 feet above ground level. Any change to the system must be done with this goal in mind. As part of the Avionics-EECS subteam, our goal is to work on the rocket's avionics systems as well as any supporting systems that move us closer to our ultimate goal.

## Basic Requirements
----------------------
The most basic requirements of a rocket avionics system are *triggering events* and *tracking the rocket*. Tracking the rocket will be how we determine if the rocket reached its goal altitude or not. There are several ways in which this step could go wrong or produce incorrect results, so redundancy and rigorous testing should be preferred. In addition to this, the rocket's avionics system must be able to trigger events under the right conditions in order to maximize the chances of reaching higher altitudes and, more importantly, the chances of successfully recovering the rocket.

## Sequence of Events
----------------------
The rocket avionics system requirements are structured around the following sequence of events:

### Pre-Launch
- Hardware Safety Check
- Configure Flight Software
- Software System Check
- Calibration

### Launch
- Send launch command
- Ignite booster
- Detect launch

### In Flight
- Record raw sensor data
- Record flight data
- Record rocket vitals (engine temperature/pressure)
- Record video
- Estimate current state (position/velocity/etc.)

### Stage Separation
- Detect booster depletion
- Ignite separation charges

### Upper-Stage Ignition
- Delay to save fuel and increase peak altitude
- Ignite sustainer

### Parachute Deployment
- Detect apogee
- Trigger chute deployment charges

### Recovery
- Transmit signal for locating the rocket once it lands
- Download flight data for further analysis

### Analysis
- Run more computationally intensive algorithms on the recorded raw sensor data to determine if the flight computer is functioning properly.
- Replay the flight in greater detail
- Use data analysis techniques to create a model of the flight
- Compare flight model to predicted/hypothesized model in order to inform future decisions & improvements

## Project Structure
----------------------
### Launch System
#### Control Box
The enclosure with the big red button

#### Launch Box
Ignites the booster when launch signal received from Control Box

### Avionics
#### Flight Computer
The hardware & software that triggers the rocket events

- TeleMegas & EasyMegas running flight software on AltOS

### Payload
#### Student-Developed Avionics
Eventually replace commercially-developed flight computer

#### Tracking Beacon
A way to track the rocket for recovery in case the flight computer’s telemetry fails

#### Camera
Record video through a window in the side of the rocket

#### Rocket Vitals
Monitor rocket internals, mostly for post-flight debugging

- Examples include motor temperature & pressure, stage-separation detection, parachute deployment detection, and dedicated state estimation

### Ground Station
#### Transceiver
Communicates with the Avionics

- Antennas
- TeleDongle

#### Ground Computer
- Configures flight software
    - AltOS
- Saves the telemetry for later use, processes the telemetry, and serves the processed data to the GUI Frontend

#### Frontend GUI
- Displays the processed data in a GUI
- Can run on Ground Computer or a computer connected to the Ground Computer
