# Ender-3-backup
A backup of the configuration files for my Ender-3 printer.
The printer is enclosed in an 1/4" acrylic chamber 24" x 24" x 36" =0.914 m 12'^
A 1000 Watt PTC heater with a Noctua 140mm hv fan heats chamber.
the printer uses LDO high temp stepper motors on all axis.
A BTT Manta E3EZ controller with a CM4-EMMC operate the printer,
along with a Rpi Pico-2350 that monitors the chamber temprature sensors.
A Sprite direct drive extruder with a CR-Touch controls the fillament.
A Fillament sensor is attached to the top cross member.

** UPDATE **
I tried to use a Rpi-pico2 2350 communicating via UART.
THIS WAS AN EPIC FAILURE. After six trial and fails, I resorted to 
USB as the best and easiest configuration for this device.

I followed: https://Github/Rootiest/guides/usb-pico.md 
ALSO: The MAX31855 sensor and the BME280 sensor have a tendency to
throw KNACK ERROR's and shutdown the MCU.
Therefore we will not be using those sensor in this build..

The MANTA E3EZ has a thermister and heater output for a second extruder,
we will be using them for the chamber heater...
