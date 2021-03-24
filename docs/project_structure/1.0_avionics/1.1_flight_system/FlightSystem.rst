Flight System
==============
The Flight System is the system of hardware & software that triggers the rocket events. For safety reasons, we are currently required to use commercially certified products to control the pyrotechnic events, but the plan is to eventually replace the commercial flight controllers with :doc:`one developed by HART <../1.2_payload/1.2.2_HART_flight_controller/FlightController>`.

Both the booster and sustainer have an Altus Metrum TeleMega and EasyMega each. The EasyMega is just a TeleMega without any RF capabilities and will be serving as a backup flight computer. Both of these systems are running AltOS. For more information about Altus Metrum products, visit the [Altus Metrum website](https://altusmetrum.org/).

.. toctree::
    :maxdepth: 3

    1.1.1_flight_hardware/FlightHardware
    1.1.2_flight_software/FlightSoftware

