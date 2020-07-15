# astropibox
Astronomy hardware/software for Raspberry PI
## Hardware
### PI Hat
#### A small PI hat
* 5 12V 
  * 4 3A-capable connectors
  * 1 3A-capabel on/off connector
  * DC Barrel jack 5.5mm 2.1mm
* 3 Temperature sensor jacks
  * 3.5mm audio jack for special temperature probes
  * DS1280 sensors
* 1 External sensor pod connector  
  * RJ-12 6 pin connector
  * Must use a 6 connector cable
* 3 Dew heater ports
  * RCA ports
  * All ports independent
* 1 Focuser port
  * RJ45 (not ethernet compatible)
  * Expected to terminate into a stepper motor
* 1 USB 3.0 port
  * To be connected to external USB3 hub
* 1 RJ-45 Ethernet port
  * Provide wired connection (wireless a good backup)
* 1 LED strip
* 1 M.2 Drive
* Autoguide port
  * Connect to the autoguide port and allow control of the mount.

### Case
### Solution
## Software
* Work with [AstroBerry](https://astroberry.io)
* Provide drivers for [INDI](https://indilib.org) 
* Provide a shim for [Alpaca-ASCOM](https://ascom-standards.org/Developer/Alpaca.htm)

