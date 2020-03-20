# SkySong XMOS XU208 Firmware


This repository contain Firmware for SkySong XMOS XU208 USB trasport.


**SkySong.bin** - version 2.20 for update with DFU.

**SkySongFull.bin** - version 2.20 which contains full SPI Flash memory dump. It can help recovery brick devices after DFU update with bad firmware. XMOS allow flash bad firmware with fine CRC(for example firmware from another devices) but after can't boot it. For recovery you need SOP8 or SPI Flash Programmer like cheap CH341 programmer with SOP8 Clip. Also you can use Raspberry PI, ESP32, STM32 and other devices with SPI interface. In internet you are can find how to connect it to SPI Flash and **Winbond W25X40** chip pins. Label of the chip may differ, so I took a photo where you are can look this chip on the board. You need to find a chip with a label **25X40** and connect it with SOP8 Clip to programmer. If there is no clip, then you can simply solder wires to the contacts. Flash this firmware and the device will work.

![CH341 Programmer](/Programmer.jpg)

![CH341 Programmer](/SkySong.jpg)
