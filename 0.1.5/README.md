# Version 0.1.5

- **emx-0.1.5.com** : "Standalone" MSX-DOS version, no need any driver, support UART 16C550  
- **emx-F0.1.5.com** : Fossil driver MSX-DOS version, needs Fossil driver
- **emx-C0.1.5.cas** and **emx-C0.1.5.wav** : Cassette version (without floppy installed)

## Usage (only for MSX-DOS versions):

`progname [speed [protocol]]`

- Without any parameter, **EMinEx** will try to detect the modem speed, using 8N1 protocol.

- With the **speed** parameter, **EMinEx** will communicate at the specified speed using the 8N1 protocol. No auto-detection.  
  Available speeds for standalone version: 57600, 38400, 19200, 14400, 9600, 4800, 2400, 1200  
  Available speeds for Fossil version: 57600, 9600, 4800, 2400, 1200

- With the **protocol** parameter, **EMinEx** will use the indicated protocol:  
  - **XYZ**:  
    - **X** = number of bits (5, 6, 7, or 8)  
    - **Y** = parity (O, E, or N)  
    - **Z** = Stop bits (1 or 2)

Cassette version will always perform auto-detection and only support UART 16C550

## Examples:

- `emx`  
- `emx 9600`  
- `emx 9600 7N1`

## Misc:
- **drv140.com** : Fossil driver 1.40 by Erik Maas 
