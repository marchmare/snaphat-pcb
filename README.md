# 🌻 SnapHAT - PCB design

![](img/snaphat.png)

SnapHAT board is a HAT (or addon) for RaspberryPi Zero 2 W combining functionalities of popular RaspberryPi-compatible modules to be serving as a handheld photo camera setup.

This repository contains KiCad 9 design files for the PCB of the SnapHAT. The board's layout is prepared to be compatible with JLCPCB standard PCB quote.

### Table of contents:

* [Features](#features)
* [Repository structure](#repository-structure)
* [Bill of Materials](#bill-of-materials)

## Features

* 40-pin Raspberry Pi GPIO header (Pi Zero 2 W compatible)
* 1200mAh Li-Po battery support (30x40mm cell footprint, 2 pin PH connector)
* integrated battery charging and power monitoring
* USB-C charging connector
* 8-pin PH connector with mounting support for 320x240 Waveshare 18366 2.4" LCD TFT display
* 8 tactile user interface buttons (navigation and shutter)
* motion sensing for automatic image orientation metadata
* passive buzzer for audio feedback
* exposed UART pins
* flower testpads, because joy and whimsy is in demand

## Repository structure

* `*.kicad_pro`, `*.kicad_sch`, `*.kicad_pcb` - KiCad 9 design files
* `docs/` - this directory contains documentation outputs generated from the KiCad files - you will find BOM in CSV format and schematic PDF in there


## Bill of Materials

> [!TIP]
> Bill of Materials for PCB assembly can be found in [this CSV file](docs/snaphat_bom.csv). 
> 
> For other components require for the setup, see tables below.

### OTS modules

| Reference | Part number | Manufacturer | Qty | Description | 
| --------- | ----------- | ------------ | --- | ----------- |
| H13 | 18366 | Waveshare | 1 | [240×320 2.4" LCD display module](https://www.waveshare.com/2.4inch-lcd-module.htm?srsltid=AfmBOopHhM1NjCceQYBKomB8Sz8IiC6UQ2W8uLNN0z1ErYVV27Lu8i5w) | 
| H14 | ODS105 | Odseven  | 1 | [OV5647 camera module for Raspberry Pi Zero](https://odseven.com/products/odseven-camera-for-raspberry-pi-zero) | 
| H15 | 10304 |  | 1 | Polymer battery, 3.7V, 1200mAh |
| H16 | SC1176 | Raspberry Pi | 1 | [Raspberry Pi Zero 2 W](https://www.raspberrypi.com/products/raspberry-pi-zero-2-w/) |

### Fasteners 

Fasteners listed take future 3D printed casing into consideration.

| Reference | Part number | Manufacturer | Qty | Description | 
| --------- | ----------- | ------------ | --- | ----------- |
| H9-H12 | 1386735 | Bossard | 4 | M2.5 threaded insert |
| H30-H32 | 970110151 | Würth Elektronik | 3 | M2.5 steel hex standoff, female-female |
| H33-H36 | 1944940 | Bossard | 4 | M1.6x4 screw |
| H37-H39 | M2.5X5/D7985 | Kraftberg | 3 | M2.5x5 screw | 
| H40-H43 | M2.5X8/D7985 | Kraftberg | 4 | M2.5x8 screw | 
| H44-H47 | M2.5X12/D7985 | Kraftberg | 4 | M2.5x12 screw | 
| H51 | 1088254 | Bossard | 1 | M2.5 nut |

### Wire harnesses

| Reference | Part number | Manufacturer | Qty | Description | 
| --------- | ----------- | ------------ | --- | ----------- |
| H17 | PHR-8 | JST | 1 | 8 position connector housing for the display | 
| H50 | PHR-2 | JST | 1 | 2 position connector housing for the battery | 
| H18-H25, H48, H49 | SPH-002T-P0.5S | JST | 10 | Metal terminal, female, for PHR housings | 




