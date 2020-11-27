# DEC RX02
Information on DEC RX01 and RX02 floppy disk drives

## RX02 FLOPPY DISK CONTROLLER
This is the controller board in the disk drive. This board connects to the interface in the computer through connector J1, to the RX02 R/W CONTROL through connector J2 and to the power supply through connector J3

### Connector J1
40 Pins IDC connection to the interface board in the computer

| Pin     | Direction*    | Function              |
|---------|---------------|-----------------------|
| A (40)  | Power         | GND                   |
| B (39)  | Power         | GND                   |
| C (38)  | Power         | GND                   |
| D (37)  | Input         | RX RUN L              |
| E (36)  | Power         | GND                   |
| F (35)  | Power         | GND                   |
| H (34)  | Power         | GND                   |
| J (33)  | Output        | RX ERROR L            |
| K (32)  | Power         | GND                   |
| L (31)  | Power         | GND                   |
| M (30)  | Power         | GND                   |
| N (29)  | Input         | RX INIT L             |
| P (28)  | Power         | GND                   |
| R (27)  | Power         | GND                   |
| S (26)  | Power         | GND                   |
| T (25)  | Output        | RX TRANSFER REQUEST L |
| U (24)  | Power         | GND                   |
| V (23)  | Power         | GND                   |
| W (22)  | Power         | GND                   |
| X (21)  | Output        | RX DONE L             |
| Y (20)  | Power         | GND                   |
| Z (19)  | Power         | GND                   |
| AA (18) | Power         | GND                   |
| BB (17) | Bidirectional | RX DATA L             |
| CC (16) | Power         | GND                   |
| DD (15) | Power         | GND                   |
| EE (14) | Power         | GND                   |
| FF (13) | Input         | RX 12 BIT L           |
| HH (12) | Power         | GND                   |
| JJ (11) | -             | NC                    |
| KK (10) | Power         | GND                   |
| LL (9)  | Output        | RX SHIFT L            |
| MM (8)  | Power         | GND                   |
| NN (7)  | Power         | GND                   |
| PP (6)  | Power         | GND                   |
| RR (5)  | Output        | RX OUT L              |
| SS (4)  | Power         | GND                   |
| TT (3)  | Output        | RX AC L               |
| UU (2)  | Power         | GND                   |
| VV (1)  | Input         | RX DMA INTF H         |

*: Direction as seen from the board.


### Connector J2

| Pin | Direction* | Function               |
|-----|------------|------------------------|
| 1   | Power      | GND                    |
| 2   | Output     | DRV OUT/ABV 43 H       |
| 3   | Output     | DRV SEL HEAD 0 H       |
| 4   | Output     | DRV ERASE H            |
| 5   | Output     | DRV WT GATE H          |
| 6   | Output     | DRV STEP L             |
| 7   | Input      | DRV READ STROBE H      |
| 8   | Output     | DRV WT DATA H          |
| 9   | Input      | DRV SEL INDX H         |
| 10  | Output     | DRV READ 2F L          |
| 11  | Output     | DRV MAINT MODE (1) H   |
| 12  | Input      | DRV SEL TRK 0 H        |
| 13  | Output     | DRV LOAD HEAD (1) H    |
| 14  | Output     | MAINTENANCE MODE (0) H |
| 15  | Output     | DRV SEL DKI H          |
| 16  | unclear    | DRV AC L               |
| 17  | Input      | DRV SEP CLK H          |
| 18  | Input      | DRV SEP DATA H         |
| 19  | Output     | DRV LOCK CLK H         |
| 20  | Power      | GND                    |

*: Direction as seen from the board.

### Connector J3

| Pin | Direction* | Function |
| 1   | Power      | +10V     |
| 2   | -          | NC       |
| 3   | Power      | GND      |
| 4   | Power      | +5V      |
| 5   | Power      | GND      |
| 6   | -          | NC       |

*: Direction as seen from the board.

## RX02 READ/WRITE CONTROL

### Connector J1
This connects to Connector J2 on the RX02 FLOPPY DISK CONTROLLER . The cable is twisted (pin 1 on one side connects to pin 20 on the other)

| Pin | Direction* | Function               |
|-----|------------|------------------------|
| 1   | Power      | GND                    |
| 2   | Input      | DRV LOCK CLK H         |
| 3   | Output     | DRV SEP DATA H         |
| 4   | Output     | DRV SEP CLK H          |
| 5   | unclear    | DRV AC L               |
| 6   | Input      | DRV SEL DKI H          |
| 7   | -          | NC                     |
| 8   | Input      | DRV LOAD HEAD (1) H    |
| 9   | Output     | DRV SEL TRK 0 H        |
| 10  | Input      | DRV MAINT MODE (1) H   |
| 11  | Input      | DRV READ 2F L          |
| 12  | Output     | DRV SEL INDX H         |
| 13  | Input      | DRV WT DATA H          |
| 14  | Output     | DRV READ STROBE H      |
| 15  | Input      | DRV STEP L             |
| 16  | Input      | DRV WT GATE H          |
| 17  | Input      | DRV ERASE H            |
| 18  | Input      | DRV SEL HEAD 0 H       |
| 19  | Input      | DRV OUT/ABV 43 H       |
| 20  | Power      | GND                    |

*: Direction as seen from the board.
