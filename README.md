STKNX Pmod
==========

**WARNING**: See [known issues](#known-issues) before ordering boards!

This is a small breakout board for an ST microelectronics [STKNX KNX line transceiver](https://www.st.com/en/interfaces-and-transceivers/stknx.html)

![PCB Front](/docs/pcb1.png)

Hardware
--------

The board is currently being manufactured and the design has briefly been powered up and tested - it didn't go up in flames... yet. It is very close to the ST reference design of the EVALKITSTKNX development board, just without the microcontroller

The STKNX is not a full KNX MAC. It is only a line transceiver that performs some KNX bus compliant signal conditioning and also delivers power using its voltage regulators from the bus to the device.

There is no real open source software support right now for bit-banging the KNX protocol using this transceiver. It is very useful to perform sniffing tasks on the bus if you are interested in the raw bits that are sent.

Known issues
------------

The polarization of the KNX connector is wrong. It's a pretty dumb mistake, but oh well, it happened.

Possible solutions:

1. Don't care, connect the red wire to the black terminal and vice versa
2. Don't care like in 1) but use the yellow/white WAGO terminal to make sure you remember to swap the polarity
3. Take apart a WAGO terminal by force and swap the black and red terminal
4. Solder the pins on the bottom of the board and plug the WAGO terminal in there.
5. Cut the GND connections on the one pin, cut the bus connection on the other pin and bodge the GND and bus connection to the right pins
6. Fix it in the board design, reorder and rebuild the boards
