<h2>The RedBoard Pro Micro-ATX</h2>

<img src="https://github.com/sparkfun/StupidArduinos/blob/master/Pro%20Micro-ATX/Stupid%20Arduino%20ATX-02.jpg?raw=true" alt="Photograph of an RGB lit side-window PC tower case housing a liquid cooler and a number of expansion cards">

Let me show you its features:

1) Convenient and well-supported Micro-ATX form factor

The Micro-ATX form factor is compatible not only with Micro-ATX PC cases but also Standard- and Extended-ATX cases. The Pro Micro-ATX conforms to the mechanical specs for footprint size, stand-off placement and expansion card position for the widest possible compatibility across case manufacturers.

2) Support for enthusiast-grade cooling hardware

The heart of the Pro Micro-ATX is an ATmega32u4 microcontroller that has been positioned (along with the necessary support components) within the mechanical footprint of an LGA 1151 socket. This gives the user a wide array of options for (pointlessly) cooling the microcontroller, including many AIO air and liquid coolers designed for modern Intel processors.

3) 24-pin ATX power support

Arguably the only useful feature on this board is the 24-pin power connector, which allows the ATmega32u4 and its peripherals to draw from any external, ATX-compatible power supply.

4) Expanded EEPROM

You may be surprised to find that I had, uh, some room on the board. I decided that one way of utilizing this space might be to stack as many I²C EEPROM chips as I could on the one available bus. That number turns out to be eight (with capacities up to 512k), giving this board a whopping 2Mbits of storage! I stopped just short of Shawn’s suggestion of laying out I²C DIMM footprints and compatible “RAM cards,” because you have to draw the line somewhere…

5) Card Slots!!!

…but NOT at expansion cards! After all, what’s a motherboard layout without expansion slots? It’s not enthusiast-grade, that’s for sure. So I created a system of expansion cards for the Pro Micro-ATX. It could be argued that the Arduino already has a system of expansion cards — shields — and that they are the best possible expansion system given that they have access to literally every I/O of the host controller. I decided that there was no electrical improvement to be made here and that, instead, adapting the shield system to the ATX form factor would be my main focus. I found the idea of using PCI connectors a little excessive, even for an undertaking of this magnitude, and opted for a smaller 28 Position Card Edge Connector. The compatible cards adapt the pinout of the edge connector back to the familiar Arduino shield form factor, so any existing shield can be connected and accessed through the expansion slots in the back of the case.

6) Rear I/O

Any good motherboard has rear I/O and the Pro Micro-ATX is no exception. Accessible from the rear panel are a standard shield footprint, a 6-pin Atmel ISP header and a USB type-B connector for serial communication.
