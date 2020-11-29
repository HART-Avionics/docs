Sequence of Events
==================
The rocket avionics system requirements are structured around the following sequence of events:

Pre-Launch
----------------------
- Hardware Safety Check
- Configure Flight Software
- Software System Check
- Calibration

Launch
----------------------
- Send launch command
- Ignite booster
- Detect launch

In Flight
----------------------
- Record raw sensor data
- Record flight data
- Record rocket vitals (engine temperature/pressure)
- Record video
- Estimate current state (position/velocity/etc.)

Stage Separation
----------------------
- Detect booster depletion
- Ignite separation charges

Upper-Stage Ignition
----------------------
- Delay to save fuel and increase peak altitude
- Ignite sustainer

Parachute Deployment
----------------------
- Detect apogee
- Trigger chute deployment charges

Recovery
----------------------
- Transmit signal for locating the rocket once it lands
- Download flight data for further analysis

Analysis
----------------------
- Run more computationally intensive algorithms on the recorded raw sensor data to determine if the flight computer is functioning properly.
- Replay the flight in greater detail
- Use data analysis techniques to create a model of the flight
- Compare flight model to predicted/hypothesized model in order to inform future decisions & improvements
