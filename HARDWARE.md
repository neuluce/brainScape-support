# brainScape Hardware

The brainScape software requires a 
[Polhemus PARTRIOT](https://polhemus.com/motion-tracking/all-trackers/patriot) 
3D digitizer to project source and detector locations onto an MR brain image.

Specifically, the following configuration is recommended:

* Polhemus PATRIOT digitizer with power adapter and serial cable for connecting to PC
* Polhemus TX1 source mounted on left side of glasses using 2 plastic screws (included with TX1 source) and connected to the SOURCE port on the Polhemus PATRIOT
* Polhemus 8-inch Stylus connected to the SENSOR1 port on the Polhemus PATRIOT
* USB to Null Modem Serial FTDI Adapter Cable to connect Polhemus PATRIOT serial port to computer USB port ([example](https://www.tripplite.com/usb-null-modem-serial-ftdi-adapter-cable-com-retention-usb-a-db9-m-f-18in~U20918NNULL/))
* Glasses (generic frames, purchased separately) onto which the TX1 is mounted

The glasses configuration is depicted in the following image:

![Image of glasses with source](https://github.com/neuluce/brainScape-support/raw/master/glasses.jpg)

## Configuring Serial Modem

The serial modem may require drivers and configuration. Install the manufacturer provided drivers, then use the Windows Device Manager to inspect the serial port configuration (under "Ports COM & LPT"). Review the following settings:

* Baud rate / Bits per second: 115200
* Data bits: 8
* Parity: none
* Stop bits: 1
* Flow control: none
* Terminator: 13
