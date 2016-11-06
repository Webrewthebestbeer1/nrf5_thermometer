## NRF5 Thermometer

This repository contains the firmware for a NRF5 with the Health Thermometer Service (HTS). The temperature is read from a DS1820 probe.

### Makefiles and paths

The Makefiles are configured to look for the nRF52 SDK at

    ~/sdk/nrf52

while the repository should be located at

    ~/git/nrf5_thermometer

The paths are relative, so any other similar structure is fine.

### Compiling and uploading firmware

First the SoftDevice has to be flashed

    make flash_softdevice

This only has to be done once per device  

Compile the firmware

    make

Compile the firmware and upload through debugger

    make flash
