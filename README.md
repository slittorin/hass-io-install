# Installation of HASS.io - 64 bit

## Prequisities

- We want a 64 bit OS to obtain speed from the RPI 4 hardware.
- Preferably, use a RPI 4 with at least 4GB RAM.
- We are following the official instructions [Install HASS.io](https://www.home-assistant.io/installation/raspberrypi).
- We want speed, stability and size compared to the built in micro-SD card, therefore we add an SSD drive to the RPI configuration.
  - We need first a suitable SSD drive, choose one that can carry load and lots of updates. I chose: Samsung 870 EVO 250GB (MZ-77E250B/EU).
  - We also need a RPI compatible SATA to USB cable, see [Compatible cables here](https://jamesachambers.com/raspberry-pi-4-usb-boot-config-guide-for-ssd-flash-drives/), I chose: StarTech USB 3.0 to 2.5" SATA HDD/SDD Cable w/UASP (USB3S2SAT3CB).

## Installation

1. First perform the steps to install RPI, as we want to upgrade the eeprom before we run HASS.io.
   - Follow the instructions here [Raspberry PI install](https://github.com/slittorin/raspberrypi-install).
     - Set hostname to: `homeassistant`.
     - You may skip all parts related to VNC.
3. Download [Balena Etcher](https://www.balena.io/etcher/).
4. Download the 64 bit image listed on [Install HASS.io](https://www.home-assistant.io/installation/raspberrypi).
5. Add the SSD Disk with the cable towards the computer.
6. 
