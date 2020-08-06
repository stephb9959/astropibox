# astropibox
Astronomy hardware/software for Raspberry PI
## Hardware
### PI Hat
#### A small PI hat
* 1 12V 10A DC Input
* 4 12V DC output 
  * 3 3A-capable connectors switchable
  * 1 3A-capabel always on
  * DC Barrel jack 5.5mm 2.1mm
* DSLR shutter control port 3.5mm
* 2 Temperature sensor jacks
  * 3.5mm audio jack for special temperature probes
  * DS1280 sensors
* 1 External sensor pod connector  
  * RJ-12 6 pin connector
  * Must use a 6 connector cable
* 2 Dew heater ports
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
### Control
#### The board has MCP23017 at address 0+default. The following bits are enabled
* GPA0: RA+
* GPA1: DEC+
* GPA2: DEC-
* GPA3: RA-
* GPA4: Switched +12v port 5
* GPA5: Sensor enable line passed to external sensor pod
* GPA6: Yellow LED
* GPA7: Green LED
* GPB0: Stepper direction
* GPB1: Stepper step
* GPB2: Stepper MS1
* GPB3: Stepper MS2
* GPB4: Stepper MS3
* GPB5: Stepper enable
#### On the RaspBerry PI, the following pins are used:
* GPIO17: dew 1 PWM
* GPIO27: dew 2 PWM
* GPIO22: dew 3 PWM
* GPIO13: temp1
* GPIO19: temp2
* GPIO26: temp3
* GPIO16: reset signal
* GPIO18: IRQ for AUX1
* GPIO23: IRQ for AUX2
* GPIO24: IRQ for AUX3
#### There is also a serial EEPROM on the board at the default address
#### AUX ports
* Use RJ25
 * Pin 1: CTS
 * Pin 2: TX
 * Pin 3: +12v
 * Pin 4: RX
 * Pin 5: GND
 * Pin 6: RTS
#### Focuser
* Uses RJ45
 * Pin 1,2: Stepper 1A
 * Pin 3,4: Stepper 1B
 * Pin 5,6: Stepper 2A
 * Pin 7,8: Stepper 2B
#### Sensor port
* Uses RJ25
 * Pin 1: GND
 * Pin 2: 3.3V
 * Pin 3: 5V
 * Pin 4: SCL
 * Pin 5: SDA
 * Pin 6: Sensor Enable

#### Autoguide
* Uses RJ25
 * Pin 1: no connection
 * Pin 2: GND
 * Pin 3: RA+
 * Pin 4: DEC+
 * Pin 5: DEC-
 * Pin 6: RA-
 


### Case
### Solution
## Software
* Work with [AstroBerry](https://astroberry.io)
* Provide drivers for [INDI](https://indilib.org) 
* Provide a shim for [Alpaca-ASCOM](https://ascom-standards.org/Developer/Alpaca.htm)

