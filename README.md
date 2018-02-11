# Purpose

NodeMCU (left) and DoIt ESP32 DevKit (right), side by side: <br>

![](https://github.com/lyusupov/SoftRF/raw/master/documents/images/ESP32-NODEMCU-ADAPTER-1.jpg)

# Pin mapping

## System

|  | 1 | 2 | 3 | 4 |
| ----------------- | -------- | -------- | -- | --- |
| NodeMCU           | GND (x4) | 3V3 (x3) | EN | VIN |
| DoIt ESP32 DevKit | GND (x2) | 3V3      | EN | VIN |

## Data

|  |1|2|3|4|5|6|7|8|9|10|11|12|13|
| ----------------- |--|--|--|--|--|--|--|--|--|---|---|--|---|
| NodeMCU           |D0|D1|D2|D3|D4|D5|D6|D7|D8|RX|TX|A0|SD3|
| DoIt ESP32 DevKit |D26|D25|D14|D23|D12|D5|D19|D27|D18|RX0|TX0|VP|D13|

## Not assigned yet

| Module | Pins |
| ----------------- | -------- |
| NodeMCU           | RST, CLK, SD0, CMD, SD1, SD2, RSV1, RSV2 |
| DoIt ESP32 DevKit | D15, D2, D4, RX2, TX2, D21, D22, D32, D33, D34, D35, VN  |

# Prototype

Prior to making a PCB design and placing an order for the manufacturing, I've soldered this prototype: <br>

![](https://github.com/lyusupov/SoftRF/raw/master/documents/images/ESP32-NODEMCU-ADAPTER-2.jpg)

It fits good enough for **SoftRF Shield**: <br> 

![](https://github.com/lyusupov/SoftRF/raw/master/documents/images/ESP32-NODEMCU-ADAPTER-3.jpg)

and for **SoftRF Enclosure V4** as well:  <br>

![](https://github.com/lyusupov/SoftRF/raw/master/documents/images/ESP32-NODEMCU-ADAPTER-4.jpg)

# PCB

TBD

# Bill of materials

TBD
