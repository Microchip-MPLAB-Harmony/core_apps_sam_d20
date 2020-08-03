[![MCHP](https://www.microchip.com/ResourcePackages/Microchip/assets/dist/images/logo.png)](https://www.microchip.com)

# Title

This example demonstrates the multi client feature of the SPI driver by performing self-loop back with two clients connected on the same SPI bus

## Description

- This example demonstrates the multi client feature of the SPI driver by reading and writing data with two clients that are connected on the same SPI bus

- It uses the request (write and read request) queuing feature of the asynchronous driver and does not waste CPU bandwidth in waiting for previous request completion

- The example also demonstrates how to setup two different client transfers at different baud rates

- This example performs self loop back only once after a power on reset

- Success is indicated when a successful self loop back is reported by both the clients

- After the loop back test is complete, the application remains in the idle state

## Downloading and building the application

To clone or download this application from Github, go to the [main page of this repository](https://github.com/Microchip-MPLAB-Harmony/core_apps_sam_d20) and then click Clone button to clone this repository or download as zip file.
This content can also be downloaded using content manager by following these [instructions](https://github.com/Microchip-MPLAB-Harmony/contentmanager/wiki).

Path of the application within the repository is **apps/driver/spi/async/spi_self_loopback_multi_client/firmware** .

To build the application, refer to the following table and open the project using its IDE.

| Project Name      | Description                                    |
| ----------------- | ---------------------------------------------- |
| sam_d20_xpro.X | MPLABX project for [SAM D20 Xplained Pro Evaluation Kit](https://www.microchip.com/developmenttools/ProductDetails/ATSAMD20-XPRO) |
|||

## Setting up the hardware

The following table shows the target hardware for the application projects.

| Project Name| Board|
|:---------|:---------:|
| sam_d20_xpro.X | [SAM D20 Xplained Pro Evaluation Kit](https://www.microchip.com/developmenttools/ProductDetails/ATSAMD20-XPRO) |
|||

### Setting up [SAM D20 Xplained Pro Evaluation Kit](https://www.microchip.com/developmenttools/ProductDetails/ATSAMD20-XPRO)

- Use jumper wire to Connect "Pin 16 of EXT2 header" to "Pin 17 of EXT2 header"

    - SERCOM1 PAD2 signal as MOSI signal and it is mapped to PA18 that is routed to "Pin 16 of EXT2 header"

    - SERCOM1 PAD0 signal as MISO signal and it is mapped to PA16 that is routed to "Pin 17 of EXT2 header"

- Connect the Debug USB port on the board to the computer using a micro USB cable

## Running the Application

1. Build and program the application using its IDE
2. The LED is turned ON on Success

Refer to the following table for LED name:

| Board | LED Name |
| ----- | -------- |
|  [SAM D20 Xplained Pro Evaluation Kit](https://www.microchip.com/developmenttools/ProductDetails/ATSAMD20-XPRO) | LED0 |
|||