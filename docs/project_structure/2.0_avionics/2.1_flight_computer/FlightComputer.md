Flight Computer
================
<!-- Block Definition -->
The Flight Computer is the hardware & software that triggers the rocket events.

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
  - Vmin: 3 V
  - Vnominal: 3.7 V
  - Vmax: 16 V

### Outputs
- Pyro Charges (External)
  - Vmin: 4 V
  - Vnominal: 12 V
  - Vmax: 16 V
- Ground Station Transceiver

Block Properties
---------------------------
We are currently required to use a commercial solution. Both the booster and sustainer have an Altus Metrum TeleMega and EasyMega each. The EasyMega is just a TeleMega without any RF capabilities and will be serving as a backup flight computer. Both of these systems are running AltOS. For more information about Altus Metrum products, visit the [Altus Metrum website](https://altusmetrum.org/).
