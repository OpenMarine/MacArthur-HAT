# MacArthur-HAT

> __Note__
>
> Kicad files will be released when the board is in production.

![MacArthur-HAT](images/macarthur-render.jpg)

After a few years of developing software for OpenPlotter, we have identified exactly what we need in terms of hardware to achieve our goals and the result is the [**MacArthur HAT**](https://shop.openmarine.net/home/23-macarthur-hat.html) (Hardware Attached on Top), an add-on board for **Raspberry Pi 4** running OpenPlotter v3. With this HAT we want to get the fully open-source boat to free ourselves from dependence on big companies and make our boats more respectful with the environment.

This name is not accidental, we want to honor [**Ellen MacArthur**](https://en.wikipedia.org/wiki/Ellen_MacArthur) who is not only known for being an exceptional sailor but also for her commitment to the [circular economy](https://ellenmacarthurfoundation.org). The MacArthur HAT is an electronic circuit that is as difficult to recycle and has an environmental cost to manufacture as any modern circuit, but it is designed to last and stay in your boat forever.

Its main function is to be able to communicate with any old or new marine electronic device using the proprietary and closed protocols **Seatalk1**, **NMEA 0183** or **NMEA 2000** and the free and open protocol **Signal K**. This means that when an on-board device dies, we are not forced to buy another of the same brand, that uses the same technology or even uses the same protocol because we can mix different devices. We will be able to recycle and reuse old devices giving them a second life or we will be able to gradually replace our old closed and proprietary models with new, cheaper, free and open ones.

You can also power the Raspberry Pi directly from the ship's batteries and it has a **smart power management system** to turn it on and off automatically and **protect the SD card**. Power can be taken directly from the CAN or Seatalk1 bus to simplify installation. This HAT is **stackable** and can be used with other HATs such as the **Moitessier HAT** or the **dAISy HAT**. It can also be connected directly to the **MAIANA AIS transponder** without the need for an adapter.

Some of the MacArthur HAT features, such as the power management, the AIS receiver/transponder, the **1-Wire sensors** or the **I2C internal and external sensors**, are optional. In this way you only buy what you need saving money and we do not have to manufacture things that will never be used saving natural resources.

MacArthur HAT is fully supported by [**OpenPlotter v3**](https://openplotter.readthedocs.io/en/latest/description/what_is_openplotter.html) and all of its features can be easily configured with just a few clicks. No drivers needed. If you are not using OpenPlotter, you can still access all its features, but you have to enable all interfaces and configure the system manually.

## Features

![MacArthur-HAT](images/macarthur-diagram.png)

- Only Raspberry Pi 4 is fully supported. If you use a Raspberry Pi 3, the NMEA 0183 inputs and outputs will not work, and you will need extra separation between the Raspberry Pi and the MacArthur HAT.
- 1x NMEA 2000 non-isolated input and output. Data connection by SPI0-1. Optional 120Ω termination resistor included. Compatible with any CAN bus.
- 2x NMEA 0183 opto-isolated inputs and 2x NMEA 0183 non-isolated outputs. Data connection by UART3 and UART5.
- 1x Seatalk1 opto-isolated input. This connector can be also used as an isolated general-purpose input.
- 1x Connector for multiple 1-Wire temperature sensors such as the DS18B20 (exhaust, engine, fridge...). A 4.7KΩ pull-up resistor is included. This connector can be also used as a non-isolated general-purpose input/output.
- 1x STEMMA QT/Qwiic connector for multiple I2C sensors (IMU, temperature, pressure, humidity, gas...). Compatible with most Adafruit and SparkFun sensors.
- Optional 12V to 5V DC/DC converter via [add-on module](https://shop.openmarine.net/home/24-power-module-for-macarthur-hat.html) to power the Raspberry Pi and its peripherals (including touch screens up to 10 inches). When you turn off the main switch of your ship, OpenPlotter will shut down safely. OpenPlotter will start cleanly when the main switch is turned on again.
- Optional GPS reception and AIS reception/transmission with the [MAIANA AIS base kit](https://shop.openmarine.net/home/15-maiana-ais-base-kit.html). The MacArthur HAT has all the features of all MAIANA AIS adapters in one. Data connection by UART0.
- Optional compass, heel, and trim via internal or external add-on module (IMU 9DOF).
- Compatible with [dAISy HAT](https://shop.openmarine.net/home/14-daisy-hat-ais-receiver.html), Moitessier HAT (hacked) and [Pypilot motor controllers](https://pypilot.org/opencart/index.php?route=product/category&path=59). Not compatible with Pypilot HAT. 
- Detachable screw connectors for easy mounting and maximum compatibility.
- Includes input and output LEDs to check activity at any time.
- No drivers needed.
