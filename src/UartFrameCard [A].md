### UART Framework Expansion Card Parts

|  # | Part                                      | RefDes  | Preferred Part Number      |
|---:|-------------------------------------------|---------|----------------------------|
|  1 | C 100nF X7R 16V (0805)                    | C1      | 478-5311-1-ND              |
|  1 | C 470nF X7R 16V (0805)                    | C2      | 1276-1199-1-ND             |
|  2 | C 1uF X7R 16V (0805)                      | C3-C4   | 1276-6471-1-ND             |
|  2 | DS LED (0805)                             | DS1-DS2 | 475-1415-1-ND              |
|  1 | F 200 mA fast (0805)                      | F1      | 507-1811-1-ND              |
|  1 | J JST XH Vertical (3w)                    | J1      | 455-2248-ND                |
|  1 | P USB C, plug, straddle 0.8mm             | P1      | WM12855-ND                 |
|  2 | R 1K 0.125W (0805)                        | R1-R2   | RMCF0805FT1K00CT-ND        |
|  1 | R 5.1K 0.125W (0805)                      | R3      | RMCF0805FT5K10CT-ND        |
|  1 | U MCP2221 (SOIC-14)                       | U1      | MCP2221-I/SL-ND            |
|  1 | VR AP2138N-3.3TRG1 (SOT23-3)              | VR1     | AP2138N-3.3TRG1DICT-ND     |


#### Board Size

|       |      Dimensions | Area    | Thickness |
|-------|-----------------|---------|-----------|
| PCB   |  24.0 x 27.9 mm | 1.1 in² |    0.8 mm |


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

For operation at 5V, the following components can be omitted:
* C3-C4
* VR1
