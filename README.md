# customizable-low-cost-aom-driver
Designed by Parker Osborne, University of San Diego

A custom low-cost four-channel RF signal generator that costs about $250 per board. Built around an Analog Devices AD9959 direct digital synthesizer, clocked and controlled by a raspberry Pi Pico 2W (RP2350). Features per channel: 9th order Nyquist image suppression filter, resistive pads for match and flatness, monolithic amplifier stage, +10 dBm delivered at SMA output. Tuned for 50-150 MHz output band.

Current Version and Notes:
The low-cost generator is currently in its first working version. A second version is currently planned, with noted changes below. This design is open source and intended to be used for atomic, molecular, and optics physics, but can be implemented in a wide variety of fields. We are currently using it for doppler cooling Rb-87 atoms to create Bose-Einstein condensates. 

Current software control is limited to basic testing functions, can be written and triggered using spare Pico GPIO pins but are not provided here.

A full proceedings paper write up is currently planned and will be added here when completed. Currently in the final testing phase of the first design.

Note: A power supply failure burnt out the synthesizer while testing in the current version. It is suggested to remove the Vsys Pin (39) from the Raspberry Pi Pico if communication over USB serial is to be used. 

Changes for Version 2:
- adding power supply protection
- adding current limiting resistor of chip select line 
- shrinking package size of capacitors in filter


  Please reach out to me if you have any questions.
