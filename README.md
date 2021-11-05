STKNX Pmod
==========

This is a small breakout board for an ST microelectronics [STKNX KNX line transceiver](https://www.st.com/en/interfaces-and-transceivers/stknx.html)

![PCB Front](/docs/pcb1.png)

Hardware
--------

The board is currently being manufactured and the design has not yet been tested in hardware. It is very close to the ST reference design of the EVALKITSTKNX development board, just without the microcontroller

The STKNX is not a full KNX MAC. It is only a line transceiver that performs some KNX bus compliant signal conditioning and also delivers power using its voltage regulators from the bus to the device.

There is no real open source software support right now for bit-banging the KNX protocol using this transceiver. It is very useful to perform sniffing tasks on the bus if you are interested in the raw bits that are sent.
