![Open Source at Morse Micro](./../images/morsemicro.png#gh-light-mode-only)
![Open Source at Morse Micro](./../images/morsemicro.png#gh-dark-mode-only)

# Welcome to Morse Micro on GitHub 

Morse Micro develops Wi-Fi HaLow silicon, software, and evaluation platforms for long-range, low-power connectivity.

## Getting Started

To get started with Morse Micro Wi-Fi HaLow check out our [Evaluation Kits](https://www.morsemicro.com/evaluation-kits/) and 
[HaLowLink Products](https://www.morsemicro.com/halowlink/), available on 
[Mouser](https://www.mouser.com/c/?m=Morse%20Micro) / [DigiKey](https://www.digikey.com.au/en/supplier-centers/morse-micro)


For desiging Wi-Fi HaLow into your own products, first check out our [Trusted Module Partners](https://www.morsemicro.com/modules/).

Official, open source software supporting these kits, products, and modules can be found in this GitHub.

Get started with the most appropriate software for your chosen evaluation kit/platform:

| Use Case | Start Here | Description |
|---|---|---|
| OpenWrt based evaluation kits, gateways, and routers | [`openwrt`](https://github.com/MorseMicro/openwrt) | Morse Micro's OpenWrt fork for building Wi-Fi HaLow gateways and routers. |
| Linux platforms | [Core Components - Linux](https://github.com/MorseMicro#core-components---linux) | Morse Micro's minimum set of software required to integrate into a Linux based platform. |
| MCU-based evaluation kits and RTOS applications | [`mm-iot-sdk`](https://github.com/MorseMicro/mm-iot-sdk), [MCU Platform Ports](https://github.com/MorseMicro#mcu-platform-ports) | Morse Micro's FreeRTOS based SDK for STM32 based evaluation kits. See available ports for extra targets. |

## Software

Morse Micro provides several software packages and ports for different development environments.

### OpenWrt

[`openwrt`](https://github.com/MorseMicro/openwrt) is the recommended Wi-Fi HaLow compatible SDK for building gateways, routers, and evaluating the Linux software stack.

This includes all of the [Linux Core Components](https://github.com/MorseMicro#core-components-linux) delivered in an [OpenWrt Feed](https://github.com/MorseMicro/morse-feed) as well as a Wi-Fi HaLow aware [`luci`](https://github.com/MorseMicro/luci) web interface.

### Core Components - Linux

A small number of software packages are required to integrate Wi-Fi HaLow into generic Linux targets.
| Repository | Description |
|---|---|
| [`morse-driver`](https://github.com/MorseMicro/morse_driver) | Morse Micro's fully-featured Linux driver. |
| [`morse-firmware`](https://github.com/MorseMicro/morse-firmware) | Morse Micro's chip firmware. |
| [`linux`](https://github.com/MorseMicro/linux) / [`rpi-linux`](https://github.com/MorseMicro/rpi-linux) | Morse Micro's patched kernels to enable full feature support |
| [`morse_cli`](https://github.com/MorseMicro/morse_cli) | Morse Micro's chip interface command line utility. |
| [`hostap`](https://github.com/MorseMicro/hostap) | Morse Micro's fork of hostap adding Wi-Fi HaLow support. |

### MM-IoT-SDK

[`mm-iot-sdk`](https://github.com/MorseMicro/mm-iot-sdk) is the primary development platform for `libmorse`, included in the SDK, targeting ARM based microcontrollers and based on FreeRTOS. `libmorse` provides a Wi-Fi HaLow MAC layer and driver for Morse Micro's chips. Use this SDK if you are evaluating Wi-Fi HaLow using the Morse Micro evaluation kits.

### MCU Platform Ports

To ease the integration of `libmorse` into a variety of different RTOS projects, Morse Micro provides a small number of platform ports.

| Port | Description |
|---|---|
| [`mm-iot-zephyr`](https://github.com/MorseMicro/mm-iot-zephyr) | A west manifest repository and west module for integration into existing [Zephyr RTOS](https://github.com/zephyrproject-rtos/zephyr) based projects |
| [`mm-iot-esp32`](https://github.com/MorseMicro/mm-iot-esp32) | [DEPRECATED] An ESP-IDF compatible port of the `mm-iot-sdk`. See instead [`halow`](https://components.espressif.com/components/morsemicro/halow) |
| [`mm-iot-cmsis`](https://github.com/MorseMicro/mm-iot-cmsis) | A CMSIS compatible packaging of the `mm-iot-sdk` to ease deployment of libmorse into a number of IDEs - notably STM32 Cube |

## Support

Support is best sought via our [community forum](https://community.morsemicro.com/).

For all documentation including user guides, application notes, hardware design files, etc. Head to our [Customer Portal](https://morsemicro.com/downloads-dashboard)

## Contributions

These repositories are provided to you, the user, to enable you to develop,
build, and integrate Wi-Fi HaLow. At the moment we are not accepting 
contributions to these repositories, but encourage you to fork, adapt, and share
your changes!
