# Espoir
<center>

![Espoir_iso](./images/hardware/espoir-angle-01.jpg)

</center>

## Overview
Espoir is a Power over Ethernet+ (PoE+ 802.3af/at) mikroBUS<sup>TM</sup> mainboard based on the ESP32-MINI-1 microcontroller. 

It reduces risk, cost, and time to market by taking care of the often more challenging aspects of designing power supply and high-speed circuits of a microcontroller board. Developers can focus on their application and get to testing and deployment quickly.

Espoir's mikroBUS<sup>TM</sup> socket provides incredible ease of use, with over 1,300 mikroBUS<sup>TM</sup> add-on boards available right away, including Connaxio's mikroShield and makroShield (coming soon<sup>TM</sup>) families.

<center>

|Example applications   |Compatible IDEs    |Compatible frameworks          |
|:----------------------|:------------------|:------------------------------|
|Smart farming          |Eclipse IDE        |Espressif's ESP-IDF            |
|Smart lighting         |PlatformIO IDE     |Arduino                        |
|Access control         |Arduino IDE        |MicroPython                    |
|Assembly line tracking |PyCharm            |ESPHome (soon<sup>TM</sup>)    |
|Home automation        |(and many more!)   |Tasmota (soon<sup>TM</sup>)    |

</center>

## Features and specifications

- ESP32-MINI-1 Processor
    - Single or dual core 240 MHz
    - 520 KB SRAM
    - 4 MB flash
- Power
    - Input: PoE+ 37 V - 57 V through the Ethernet connector, with 2,250 V isolation
    - Input: 5 V through the USB-C connector (4.6 V available through a protection diode)
    - Output: 5 V at 3 A (15 W) from PoE
    - Output: 3.3 V at 0.7 A (2.3 W) (Linear, derived from the 5 V power rail)
    - Jumper-selectable PoE Class 2, 3, and 4
    - Pi-filtered PoE input and output
    - Overload and thermal protections 
- Connectivity
    - Wifi 2.4 GHz 802.11b/g/n \& integrated antenna
    - Bluetooth 4.2 BLE
    - Ethernet 10/100-BaseT (80+ mbps throughput)
    - USB 2.0 via USB-C connector (tested at 2 MBaud)
    - Full mikroBUS<sup>TM</sup> socket with two grounds, 5 V, 3.3 V and 12 IOs
    - Extension header with two grounds, four additional input only pins, and the ESP32 reset signal (unsoldered socket header included)
- Mechanical
    - Weight: 31 g
    - Size: 50.8 x 61.0 mm<sup>2</sup>
    - PCB thickness: 1.6 mm
    - Four copper layers provide augmented thermal dissipation and electromagnetic compatibility
    - Mounting holes: 4x M2.5 / 4-40. The bottom-left hole is plated and connected to local ground.
- Operating temperature range: -40 <sup>o</sup>C to +85 <sup>o</sup>C

## Top and bottom views
<center>

![Espoir_top_bottom](./images/hardware/espoir-front-back-01.jpg)

</center>


## Pinout
<center>

![Espoir_pinout](./images/hardware/espoir_pinout.jpg)

</center>


## Dimensions
The main dimensions of Espoir are presented here. Complete 3D models can be found in Espoir's repository on Github.

<center>

![Espoir_dimensions](./images/hardware/espoir_dimensions.jpg)

</center>



The connector shields and the bottom-left mounting hole are connected to the local ground. It is therefore safe (and recommended) to connect them to a metal case.

Care must be taken to leave enough spacing under the PCB to avoid accidental contact of the through-hole pins with the case. A 1 mm gap should be observed between the pins and and any conductive material to maintain proper isolation. 3 mm between the bottom of the PCB and the mounting surface is typically a good starting point.

## Safety considerations
### Electrocution hazard
The area around the main transformer and Ethernet jack contains parts that operate at a typical voltage of 57 V, with peak voltages of up to 150 V. In some situations, these voltages may cause injury or death. Avoid contact with the SMD components (top) or solder joints (bottom) during operation.

### Burn hazard
Under constant heavy load, the area and parts around the main transformer may reach over 100 <sup>o</sup>C and cause severe burns. Avoid contact with both the top and bottom of the PCB in that region when high load conditions are expected.

### Safe handling
An IP20 enclosure with proper ventilation is recommended to avoid accicental contact and overheating. Espoir's repository offers a 3D printable snap-on backplate that provides protection from accidental contact and good ventilation.

## Certifications
<center>

|Directive  |Applicable standards   |
|:----------|:----------------------|

</center>

## Additional resources
- [Espoir's page on Connaxio's website](https://www.connaxio.com/electronics/espoir/)
- [Espoir's source on GitHub](https://github.com/Connaxio/espoir)
- [Espoir's launch page at Crowd Supply](https://www.crowdsupply.com/connaxio/espoir)
- [Espoir's OSHWA certification page](https://certification.oshwa.org/ca000009.html)
- [Datasheet: ESP32-MINI-1](https://www.espressif.com/sites/default/files/documentation/esp32-mini-1_datasheet_en.pdf)
- [Datasheet: ESP32-U4WDH](https://www.espressif.com/sites/default/files/documentation/esp32_datasheet_en.pdf)
- [Connaxio's Twitter handle](https://twitter.com/connaxio)
- [Connaxio's page on LinkedIn](https://www.linkedin.com/company/connaxio/)



