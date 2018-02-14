# Purpose

NodeMCU (left) and DoIt ESP32 DevKit (right), side by side: <br>

![](https://github.com/lyusupov/SoftRF/raw/master/documents/images/ESP32-NODEMCU-ADAPTER-1.jpg)

# Pin mapping

## System

|  | 1 | 2 | 3 | 4 |
| ----------------- | -------- | -------- | -- | --- |
| NodeMCU           | GND (x4) | 3V3 (x3) | EN | VIN |
| DoIt ESP32 DevKit | GND (x2) | 3V3      | EN | VIN |

## Data. Bank 1. In use by SoftRF firmware.

|  |1|2|3|4|5|6|7|8|9|10|11|12|13|
| ----------------- |--|--|--|--|--|--|--|--|--|---|---|--|---|
| NodeMCU           |D0|D1|D2|D3|D4|D5|D6|D7|D8|RX|TX|A0|SD3|
| DoIt ESP32 DevKit |D26|D25|D14|D23|D12|D5|D19|D27|D18|RX0|TX0|VP|D13|

## Data. Bank 2. Spare pins.

|  |1|2|3|4|5|6|7|8|
| ----------------- |--|--|--|--|--|--|--|--|
| NodeMCU           |RSV1|RSV2|SD1|SD2|CLK|CMD|SD0|RST|
| DoIt ESP32 DevKit |RX2|TX2|D21|D22|D15|D4|D2|VN|

## Optional J1 connector. Residual ESP32 pins and UAV (MAVLINK) port.

|1|2|3|4|5|6|
|--|--|--|--|--|--|
|3V3|GND|D32|D33|D34|D35|


## Optional J2 connector. NRF905 or "SoftRF LoRA" port.

TBD

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
