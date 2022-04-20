[UartWork](https://medo64.com/uartwork/)
========================================

This Framework laptop expansion card will show up on your system as a serial
device and allow for a non-isolated serial UART communication up to 115,200
baud rate at 3.3V.

Please note that this card is not using RS-232 but TTL (3.3V) voltage levels.


## UART Pinout

| # | Ref | Description                     |
|--:|-----|---------------------------------|
| 1 | RXD | Receive (TTL 3.3V)              |
| 2 | GND | Ground connection               |
| 3 | TXD | Transmit (TTL 3.3V)             |

PS: Colors are just a suggestion and it's not necessary to have them match the
table.


### Wiring

To connect to this board, one has to use a 3-pin JST XH connector. The following
table represents the pinout, pin 1 being on the left as looking into the
expansion card.

As power consumption is way below 10 mA, wires can be almost any AWG. I would
recommend using 24 AWG wire 0.25 mm² as they allow for greater compatibility
with other connectors.

---
*You can check my blog and other projects at [www.medo64.com](https://www.medo64.com/electronics/).*
