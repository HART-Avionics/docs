HART Flight Computer
=====================
<!-- Block Definition -->
The HART Flight Computer is the student-developed flight computer currently under development.

Interface Definitions & Properties
-----------------------------------
### Inputs
- Environment (External)
  - Acceleration
    - Max: 50 G
  - Altitude
  - Attitude (pose/orientation)
  - GPS data
  - Magnetic Field
  - Temperature
- Power Systems
  - Vmin: 3.3 V
  - Vnominal: 3.7 V
  - Vmax: 16 V

### Outputs
- Ground Station GUI Server
  - Flight data structure matches AltOS data structure

Block Properties
-----------------
We are currently required to use commercially available products to control the rocket events, but the plan is to eventually replace the commercially-developed flight computers with a student-developed solution.
