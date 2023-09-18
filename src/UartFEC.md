### UartIsoFEC Parts

|  # | Part                                              | RefDes  | Preferred Part Number       |
|---:|---------------------------------------------------|---------|-----------------------------|
|  1 | C 10nF X7R 16V (0805)                             | C1      | 399-17617-1-ND              |
|  2 | C 100nF X7R 16V (0805)                            | C2-C3   | 478-5311-1-ND               |
|  1 | C 4.7uF X5R 16V (0805)                            | C4      | 1276-1244-1-ND              |
|  1 | D TVS 5V SM05T1G (SOT23-3)                        | D1      | SM05T1GOSCT-ND              |
|  2 | DS LED (0805)                                     | DS1-DS2 | 475-1415-1-ND               |
|  1 | J JST XH Vertical (3w)                            | J1      | 455-2248-ND                 |
|  1 | L Ferrite 600R@100Mhz                             | L1      | 240-2390-1-ND               |
|  2 | R 1K 0.125W (0805)                                | R1-R2   | RMCF0805FT1K00CT-ND         |
|  1 | R 5.1K 0.125W (0805)                              | R6      | RMCF0805FT5K10CT-ND         |
|  1 | U Transciever Uart FT232R (SSOP-28)               | U1      | 768-FT232RNQ-REELCT-ND      |


#### Board Size

|       |      Dimensions | Area    | Thickness |
|-------|-----------------|---------|-----------|
| PCB   |  24.0 x 27.9 mm | 1.1 in² |    0.8 mm |


#### FTDI Configuration

| Setting | Value  |
|---------|--------|
| CBUS0   | TXDEN  |
| CBUS1   | RXLED# |
| CBUS2   | TXLED# |
| CBUS3   | PWREN# |


#### Power

| Property | Value  |
|----------|-------:|
| Voltage  |    5 V |
| Current  | 100 mA |


#### Jumpers

##### 3V3

This jumper has to be bridged for operation in 3.3V. If this jumper is bridged,
5V jumper MUST NOT be bridged too.

##### 5V

This jumper has to be bridged for operation in 5V. If this jumper is bridged,
3.3V jumper MUST NOT be bridged too.
