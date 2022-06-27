### UART Framework Expansion Card Parts

|  # | Part                                      | RefDes  | Preferred Part Number      |
|---:|-------------------------------------------|---------|----------------------------|
|  1 | C 100nF X7R 16V (0805)                    | C1      | 478-5311-1-ND              |
|  1 | C 100nF X7R 16V (0805) `NOT POPULTED`     | C2      | 478-5311-1-ND              |
|  1 | C 470nF X7R 16V (0805)                    | C3      | 1276-1199-1-ND             |
|  2 | C 1uF X7R 16V (0805)                      | C4-C5   | 1276-6471-1-ND             |
|  1 | C 10uF X5R 25V (0805) `I2C ONLY`          | C6      | 587-2985-1-ND              |
|  1 | D Shottky 30V 800 mA (SOD323) `I2C ONLY`  | D1      | CUS08F30H3FCT-ND           |
|  2 | DS LED (0805)                             | DS1-DS2 | 475-1415-1-ND              |
|  1 | F 200 mA fast (0805)                      | F1      | 507-1811-1-ND              |
|  1 | F 200 mA fast (0805) `I2C ONLY`           | F2      | 507-1811-1-ND              |
|  1 | J JST XH Vertical (3w)                    | J1      | 455-2248-ND                |
|  1 | J JST XH Vertical (7w) `ALTERNATE (I2C)`  | J1      | 455-2252-ND                |
|  1 | P USB C, plug, straddle 0.8mm             | P1      | WM12855-ND                 |
|  2 | R 3K3 0.125W (0805)                       | R1-R2   | RMCF0805FT3K30CT-ND        |
|  2 | R 3K3 0.125W (0805) `I2C ONLY`            | R3-R4   | RMCF0805FT3K30CT-ND        |
|  1 | R 5.1K 0.125W (0805)                      | R5      | RMCF0805FT5K10CT-ND        |
|  1 | U MCP2221 (SOIC-14)                       | U1      | MCP2221-I/SL-ND            |
|  1 | U AT30TS74-XM8M-T (MSOP-8) `NOT POPULTED` | U2      | AT30TS74-XM8M-TCT-ND       |
|  1 | VR AP2138N-3.3TRG1 (SOT23-3)              | VR1     | AP2138N-3.3TRG1DICT-ND     |


#### Board Size

|       |      Dimensions | Area    | Thickness |
|-------|-----------------|---------|-----------|
| PCB   |  24.0 x 27.9 mm | 1.1 in² |    0.8 mm |


#### Power

| Property | Value  |
|----------|-------:|
| Voltage  |    5 V |
| Current  | 200 mA |


#### Jumpers

##### 3V3

This jumper has to be bridged for operation in 3.3V. If this jumper is bridged,
5V jumper MUST NOT be bridged too.

##### 5V

This jumper has to be bridged for operation in 5V. If this jumper is bridged,
3.3V jumper MUST NOT be bridged too.

For operation at 5V, the following components can be omitted:
* C3-C4
* VR1


#### Pull-up Resistors

This board uses 3.3KΩ pull-up resistors out of box.

It's really hard to get an universal pull-up resistor values when it's not
known ahead of time what capacitance will I2C bus end up with. Considering
this device is intended for testing I2C, I trust 3.3KΩ is low enough to
allow for decent bus capacitance while also high enough not to mess with
devices.

However, this is just a starting point and changing pull-up resistors (either
with higher or lower values) is sometime necessary.


#### Optional I2C Sensor

If one wants to have a sensor to test I2C communication without having to
connect external devices, C2 and U2 should be populated.
