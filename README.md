# Installation of HASS.io - 64 bit

## Prequisities

- We want a 64 bit OS to obtain speed from the RPI 4 hardware.
- Preferably, use a RPI 4 with at least 4GB RAM.
- We are following the official instructions [Install HASS.io](https://www.home-assistant.io/installation/raspberrypi).
- We want speed, stability and size compared to the built in micro-SD card, therefore we add an SSD disk to the RPI configuration.
  - We need first a suitable SSD disk, choose one that can carry load and lots of updates. I chose: Samsung 870 EVO 250GB (MZ-77E250B/EU).
  - We also need a RPI compatible SATA to USB cable, see [Compatible cables here](https://jamesachambers.com/raspberry-pi-4-usb-boot-config-guide-for-ssd-flash-drives/), I chose: StarTech USB 3.0 to 2.5" SATA HDD/SDD Cable w/UASP (USB3S2SAT3CB).

## Installation of SSD disk, RPI and HASS.io

1. First perform the steps to install RPI, as we want to upgrade the eeprom before we install HASS.io.
   - Follow the instructions [Raspberry PI install](https://github.com/slittorin/raspberrypi-install).
     - Set hostname to: `homeassistant`.
     - Do not set VNC options, do not install docker and no need to fine tune installation.
2. Shutdown and remove power from the RPI.
4. Remove the micro-SD Card on the RPI (keep it preferably in the RPI but not fully inserted, or attached to the RPI).
5. Download [Balena Etcher](https://www.balena.io/etcher/).
6. Download the 64 bit image listed on [Install HASS.io](https://www.home-assistant.io/installation/raspberrypi).
7. Add the SSD disk to the computer.
8. Run Etcher and write the downloaded HASS.io-image to the SSD-disk.
9. Remove the SSD disk from the computer.
10. Add the SSD disk to the RPI.
11. Add power to the RPI.
12. Wait for 10 minutes (how long time is needed?).
13. In a web browser go the IP address (or hostname) and port 8123, for example [http://192.168.2.20:8123/](http://192.168.2.20:8123/).
14. Perform the [onboarding procedure](https://www.home-assistant.io/getting-started/onboarding/).

Continue in [Home Assistant setup](https://github.com/slittorin/home-assistant-setup).
