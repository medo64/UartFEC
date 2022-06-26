[UART+I2C Framework Expansion Card](https://medo64.com/uartframecard/)
======================================================================

This Framework laptop expansion card will show up on your system as both serial
and HID device.

Using serial device will allow for a non-isolated serial UART communication with
baud rate up to 115,200  at 3.3V. Please note that this card is not using RS-232
but TTL (3.3V) voltage levels.

I2C device will allow for non-isolated serial I2C communication up to 400 kHz
clock rate supports both 7-bit or 10-bit addressable devices. USB is not ideal
protocol for I2C communication due to how transfers are handled and thus your
I2C bandwidth will be severly limited.


## UART+I2C Pinout

| # | Ref | Description                                |
|--:|-----|--------------------------------------------|
| 1 | SDA | I2C data signal (TTL 3.3V / 3.3K pull-up)  |
| 2 | SCL | I2C clock signal (TTL 3.3V / 3.3K pull-up) |
| 3 | RXD | UART receive (TTL 3.3V)                    |
| 4 | GND | Ground connection                          |
| 5 | TXD | UART transmit (TTL 3.3V)                   |
| 6 |  -  | Not connected                              |
| 7 | V+  | Voltage output; DO NOT exceed 100 mA       |


## Wiring

To connect to this board, one has to use a 7-pin JST XH connector. The following
table represents the pinout, pin 1 being on the left as looking into the
expansion card.

As power consumption is way below 10 mA on signal lines and only up to 100 mA on
power lines, wires can be almost any AWG. I would recommend using 24 AWG wire
0.25 mm² as they allow for greater compatibility with other connectors.

---
*You can check my blog and other projects at [www.medo64.com](https://www.medo64.com/electronics/).*
