# RPi Recalbox Arcade Control Interface Module
This is a Kicad project of a PCB design for a DIY Arcade system. The goal was to design a PCB that could be easily connected to buttons via JST connectors and the standard Raspberry Pi 40-Pin GPIO header. This is a two layer board with the Top Copper layer being the main signal layer and the bottom board being the ground plane.

## Bill of Materials
| Item         | Qty       |Part Number           |
|--------------|-----------|----------------------|
| JST-XH 4-Pin | 7         |S4B-XH-SM4-TB(LF)(SN) |
| IDT 40-Pin   | 1         |SBH11-PBPC-D20-ST-BK  |

## PCB Render
![Board Render](https://github.com/roycepope/rpi-arcade-hat/blob/main/pics/render.png?raw=true)

## RecalBox GPIO Map
```bash
# button control: Y-, Y +, X-, X +, start, select, a, b, tr, y, x, tl
map=1 gpio=pin5,pin3,pin7,pin8,pin15,pin16,pin10,pin11,pin19,pin13,pin12,pin18
map=1,2 gpio=pin24,pin23,pin26,pin29,pin36,pin37,pin31,pin32,pin40,pin35,pin33,pin38
```

|GPIO#  |Pin#       |Control               |  |GPIO#  |Pin#   |Control               |
|-------|-----------|----------------------|--|-------|-------|----------------------|
| 2     | 3         | Player 1 Up          |  |11     | 23    | Player 2 Up          |
| 3     | 5         | Player 1 Down        |  | 8     | 24    | Player 2 Down        |
| 4     | 7         | Player 1 Left        |  | 7     | 26    | Player 2 Left        |
| 14    | 8         | Player 1 Right       |  | 5     | 29    | Player 2 Right       |
| 15    | 10        | Player 1 A           |  | 6     | 31    | Player 2 A           |
| 17    | 11        | Player 1 B           |  | 12    | 32    | Player 2 B           |
| 18    | 12        | Player 1 X           |  | 13    | 33    | Player 2 X           |
| 27    | 13        | Player 1 Y           |  | 19    | 35    | Player 2 Y           |
| 22    | 15        | Player 1 Start       |  | 16    | 36    | Player 2 Start       |
| 23    | 16        | Player 1 Select(Coin)|  | 26    | 37    | Player 2 Select(Coin)|
| 24    | 18        | Player 1 L1          |  | 20    | 38    | Player 2 L1          |
| 10    | 19        | Player 1 R1          |  | 21    | 40    | Player 2 R1          |







