---
parent: Harmony 3 driver and system service application examples for SAM D20 family
title: I2C EEPROM AT24 driver - EEPROM Read Write 
has_children: false
has_toc: false
---

[![MCHP](https://www.microchip.com/ResourcePackages/Microchip/assets/dist/images/logo.png)](https://www.microchip.com)

# I2C EEPROM AT24 driver - EEPROM Read Write

This example application demonstrates how to use the AT24 driver to perform read and write operations on AT24 series of EEPROM. 

## Description

This example uses the AT24 driver to communicate with the I2C based AT24 series of EEPROMs to perform read and write operations. 

The application communicates with the [EEPROM 3 click board](https://www.mikroe.com/eeprom-3-click) that has AT24CM02 EEPROM on it.

## Downloading and building the application

To clone or download this application from Github, go to the [main page of this repository](https://github.com/Microchip-MPLAB-Harmony/core_apps_sam_d20) and then click Clone button to clone this repository or download as zip file.
This content can also be downloaded using content manager by following these [instructions](https://github.com/Microchip-MPLAB-Harmony/contentmanager/wiki).

Path of the application within the repository is **apps/driver/i2c_eeprom/at24/at24_eeprom_read_write/firmware** .

To build the application, refer to the following table and open the project using its IDE.

| Project Name      | Description                                    |
| ----------------- | ---------------------------------------------- |
| sam_d20_xpro.X | MPLABX project for [SAM D20 Xplained Pro Evaluation Kit](https://www.microchip.com/developmenttools/ProductDetails/ATSAMD20-XPRO) |
|||

- To run the demo, the following additional hardware are required:
    - [EEPROM 3 click board](https://www.mikroe.com/eeprom-3-click)
    - [mikroBUS Xplained Pro board](https://www.microchip.com/developmenttools/ProductDetails/ATMBUSADAPTER-XPRO)

## Setting up the hardware

The following table shows the target hardware for the application projects.

| Project Name| Board|
|:---------|:---------:|
| sam_d20_xpro.X | [SAM D20 Xplained Pro Evaluation Kit](https://www.microchip.com/developmenttools/ProductDetails/ATSAMD20-XPRO) |
|||

### Setting up [SAM D20 Xplained Pro Evaluation Kit](https://www.microchip.com/developmenttools/ProductDetails/ATSAMD20-XPRO)

- Install an [EEPROM 3 click board](https://www.mikroe.com/eeprom-3-click) on to the [mikroBUS Xplained Pro board](https://www.microchip.com/developmenttools/ProductDetails/ATMBUSADAPTER-XPRO)

- Connect the [mikroBUS Xplained Pro board](https://www.microchip.com/developmenttools/ProductDetails/ATMBUSADAPTER-XPRO) to the EXT2 header of the [SAM D20 Xplained Pro Evaluation Kit](https://www.microchip.com/developmenttools/ProductDetails/ATSAMD20-XPRO)

- Connect the Debug USB port on the board to the computer using a micro USB cable

## Running the Application

1. Build and program the application using its IDE.
2. The LED indicates the success or failure.
    - The LED is turned ON when the data read from EEPROM matches with the written data

Refer to the following table for LED name:

| Board | LED Name |
| ----- | -------- |
|  [SAM D20 Xplained Pro Evaluation Kit](https://www.microchip.com/developmenttools/ProductDetails/ATSAMD20-XPRO) | LED0 |
|||