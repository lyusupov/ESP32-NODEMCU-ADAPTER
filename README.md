* [Purpose](https://github.com/lyusupov/ESP32-NODEMCU-ADAPTER#purpose)
* [Pin mapping](https://github.com/lyusupov/ESP32-NODEMCU-ADAPTER#pin-mapping)
* [Adapter](https://github.com/lyusupov/ESP32-NODEMCU-ADAPTER#adapter)
* [PCB](https://github.com/lyusupov/ESP32-NODEMCU-ADAPTER#pcb-manufacturing)
* [BOM](https://github.com/lyusupov/ESP32-NODEMCU-ADAPTER#bill-of-materials)
* [Errata](https://github.com/lyusupov/ESP32-NODEMCU-ADAPTER#errata)

# Purpose

NodeMCU (left) and DoIt ESP32 DevKit (right), side by side: <br>

![](https://github.com/lyusupov/SoftRF/raw/master/documents/images/ESP32-NODEMCU-ADAPTER-1.jpg)

# Pin mapping

## System

|  | 1 | 2 | 3 | 4 |
| ----------------- | -------- | -------- | -- | --- |
| NodeMCU           | GND (x4) | 3V3 (x3) | EN | VIN |
| DoIt ESP32 DevKit | GND (x2) | 3V3      | EN | VIN |

## GPIO. Bank 1. In use by SoftRF firmware.

|  |1|2|3|4|5|6|7|8|9|10|11|12|13|
| ----------------- |--|--|--|--|--|--|--|--|--|---|---|--|---|
| NodeMCU           |D0|D1|D2|D3|D4|D5|D6|D7|D8|RX|TX|A0|SD3|
| DoIt ESP32 DevKit |D26|D25|D14|D23|D2|D5|D19|D27|D18|RX0|TX0|VP|D13|

## GPIO. Bank 2. Spare pins.

|  |1|2|3|4|5|6|7|8|
| ----------------- |--|--|--|--|--|--|--|--|
| NodeMCU           |RSV1|RSV2|SD1|SD2|CLK|CMD|SD0|RST|
| DoIt ESP32 DevKit |RX2|TX2|D21|D22|D15|D4|D12|VN|

## UAV connector (optional). Residual ESP32 pins and GNSS/MAVLINK port.

|  |1|2|3|4|5|6|7|
|--|--|--|--|--|--|--|--|
| 2 |A0|D1|RX|TX|D3|GND|5V|
| 1 |3V3|GND|D32|D33|D34|D35|SD3|

## RF connector (optional). NRF905 or "SoftRF LoRa" port.

|  |1|2|3|4|5|6|7|
|--|--|--|--|--|--|--|--|
| 2 |D0|D2|D35|D34|D7|D8|GND|
| 1 |3V3|D4|NC|NC|D6|D5|GND|

# Adapter

<p><img src="https://github.com/lyusupov/SoftRF/raw/master/documents/images/ESP32-NODEMCU-ADAPTER-5.jpg" width="40%" height="40%"> <img src="https://github.com/lyusupov/SoftRF/raw/master/documents/images/ESP32-NODEMCU-ADAPTER-6.jpg" width="40%" height="40%"></p>

It fits good enough for **SoftRF Shield**: <br> 

<p><img src="https://github.com/lyusupov/SoftRF/raw/master/documents/images/ESP32-NODEMCU-ADAPTER-8.jpg" width="40%" height="40%"> <img src="https://github.com/lyusupov/SoftRF/raw/master/documents/images/ESP32-NODEMCU-ADAPTER-7.jpg" width="40%" height="40%"></p>

and for **SoftRF Enclosure V4** as well:  <br>

![](https://github.com/lyusupov/SoftRF/raw/master/documents/images/ESP32-NODEMCU-ADAPTER-9.jpg)

# PCB manufacturing

You can order the PCB direct from manufacturer: <sup>1</sup>

&nbsp;&nbsp;&nbsp;&nbsp; <a href="https://PCBs.io/share/4xgbg"><img src="https://s3.amazonaws.com/pcbs.io/share.png" alt="Order from PCBs.io"></img></a><br>

Estimated price for minimum 4 pcs of the PCB with basic international shipping included in is around 7 USD.<br>

Expect to wait:
- 1 week for panelization
- 2 weeks for fabrication 
- 1-2 weeks for delivery to your location

Alternatively you may pick [these Gerber files](https://github.com/lyusupov/ESP32-NODEMCU-ADAPTER/raw/master/gerber/ESP32-NODEMCU-ADAPTER-v1.1.zip) and order the PCB from a local manufacturer of your preference.

<sup>1</sup> - SSL Cert error warning may come up - it is known to be safely ignored<br>
<br>

![](https://github.com/lyusupov/SoftRF/raw/master/documents/images/ESP32-NODEMCU-ADAPTER-PCB.JPG)

# Bill of materials

Number|Part|Qty|Picture|Source
---|---|---|---|---
1|PCB|1|![](https://s3.amazonaws.com/pcbsio/svgs/e35706dacc5c602ce8189f8155dde1864330ef9521bdc46b84b4bb962c59313d/top.svg)|<a href="https://PCBs.io/share/4xgbg"><img src="https://s3.amazonaws.com/pcbs.io/share.png" alt="Order from PCBs.io"></img></a>
2|1x40 female header 2.54mm|1|![](https://github.com/lyusupov/SoftRF/blob/master/documents/images/bom/f1x40.jpg)|[AliExpress](https://www.aliexpress.com/item/10-2-54-40/32839452712.html)
3|1x40 male header 2.54mm|1|![](https://github.com/lyusupov/SoftRF/blob/master/documents/images/bom/m40.jpg)|[AliExpress](https://www.aliexpress.com/item/10pcs-40-Pin-1x40-Single-Row-Male-2-54-Breakable-Pin-Header-Connector-Strip-for-Arduino/32806313091.html)

# Errata

## Revision 1.1
### Issue #1
[Unable to update ESP32's firmware via micro USB when an I2C device is connected to SoftRF LoRa I2C port](https://github.com/lyusupov/ESP32-NODEMCU-ADAPTER/issues/2)

### Issue #2
[Standalone Edition/ESP32 is unable to boot up when running on 2 fully charged AA Ni-Mh 1.2V batteries with DC-DC up-converter](https://github.com/lyusupov/ESP32-NODEMCU-ADAPTER/issues/3)

<!--
## Revision 1.0

### Issue
[ESP32 does not boot when an I2C device is connected to SoftRF LoRa I2C port](https://github.com/lyusupov/ESP32-NODEMCU-ADAPTER/issues/1)
-->
