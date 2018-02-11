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

|  | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 | 11 | 12 | 13 |
| ----------------- | -- | -- | -- | -- | -- | -- | -- | -- | -- | --- | --- | -- | --- |
| NodeMCU           | D0 | D1 | D2 | D3 | D4 | D5 | D6 | D7 | D8 | RX  | TX  | A0 | SD3 |
| DoIt ESP32 DevKit | 26 | 25 | 14 | 23 | 12 |  5 | 19 | 27 | 18 | RX0 | TX0 | VP |  13 |

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
