# RP2040v01 - RP2040 Processor Module
## Introduction

The [MLAB](https://www.mlab.cz/) module RP2040v01 featuring the [RP2040](https://www.raspberrypi.com/documentation/microcontrollers/rp2040.html) processor is a powerful and flexible development board designed for a wide range of applications. The [RP2040](https://www.raspberrypi.com/documentation/microcontrollers/rp2040.html), a microcontroller from the Raspberry Pi Foundation, offers dual Arm Cortex-M0+ cores and extensive peripheral support.

![RP2040v01 Image](doc/gen/img/RP2040v01-top.png)

## Features

- **Processor**: Dual-core Arm Cortex-M0+ [RP2040](https://www.raspberrypi.com/documentation/microcontrollers/rp2040.html).
- **Buttons**: Boot and Reset buttons for easy programming and reset.
- **GPIO**: Processor pins are exposed on doubleheader pins for flexible connectivity, as is usual in MLAB modules.
- **LED**: An LED connected via a transistor on pin 25 for status indication.
- **USB**: USB-C connector for power and data communication.
- **Power Management**: Integrated power converter to step down from 5V to 3.3V.

## Processor Details

The RP2040 processor, developed by the Raspberry Pi Foundation, is a versatile microcontroller that includes the following key features:

- **Architecture**: Dual-core Arm Cortex-M0+.
- **Clock Speed**: Up to 133 MHz.
- **Memory**: 264KB of SRAM, and support for up to 16MB of external QSPI flash memory.
- **GPIO**: 30 GPIO pins, including a rich set of I/O options like UART, SPI, I2C, PWM, and ADC.
- **Timers**: Multiple timers and a real-time clock (RTC).
- **DMA**: Direct Memory Access controller for efficient data transfer.
- **Debugging**: SWD (Serial Wire Debug) interface for debugging and development.

## Programming Options

The RP2040 microcontroller offers multiple programming options, providing flexibility for various types of developers:

1. **MicroPython**:
   - An easy-to-use Python interpreter ideal for beginners.
   - Allows rapid prototyping and development with an extensive set of libraries.
   - [Official documentation](https://datasheets.raspberrypi.com/pico/raspberry-pi-pico-python-sdk.pdf)


2. **C/C++ with the Pico SDK**:
   - Provides low-level access to the hardware for maximum performance.
   - Suitable for more complex projects and experienced developers.
   - Requires setting up the Pico SDK and toolchain on your development environment.
   - [User-friendly documentation](https://datasheets.raspberrypi.com/pico/raspberry-pi-pico-c-sdk.pdf)

3. **Arduino IDE**:
   - Offers a familiar environment for those used to Arduino development.
   - Supports both the Mbed OS core and the C/C++ SDK-based core.
   - Simplifies the process of writing, compiling, and uploading sketches to the RP2040.
   - [Documentation](https://github.com/earlephilhower/arduino-pico)

### Drag-and-Drop Programming:
   - Allows you to upload firmware by simply dragging and dropping a UF2 file.
   - Useful for quick updates and easy deployment without needing an IDE.
   - Minimal knowledge required, best for beginners.

## Usage

1. **Flashing Firmware**:
   - Hold the Boot button and press the Reset button.
   - Release the Reset button while still holding the Boot button to enter bootloader mode.
   - Drag and drop the firmware file onto the USB drive that appears.

2. **Programming**:
   - Use your preferred IDE (e.g., Thonny, VS Code, Arduino IDE) and select the appropriate board and port.
   - Write your code and upload it to the RP2040.

## References
 - **PR2040** [documentation page](https://www.raspberrypi.com/documentation/microcontrollers/rp2040.html)


## Examples

Example code and projects can be found in the `examples` directory of the repository. These include basic GPIO manipulation, sensor interfacing, and communication protocols.


## Module Schematic

The schematic of the RP2040v01 module illustrates the connections and components used in the design. This includes the layout of the RP2040 processor, power management circuitry, and GPIO pin headers.

[![](doc/gen/RP2040v01-schematic.svg)](doc/gen/RP2040v01-schematic.pdf)

This README provides a comprehensive overview of the RP2040v01 module, detailing its features, setup, and usage instructions, along with an in-depth look at the RP2040 processor's capabilities and the module's schematic. For further details, consult the example codes and internal documentation.
