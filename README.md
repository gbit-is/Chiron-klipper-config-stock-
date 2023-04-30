# Chiron-klipper-config-stock

A basic config for a stock anycubic chiron to use klipper. (stock except it has a 0.6 nozzle)

As of writing this, this config is running on:
- klipper v0.11.0-148
- Raspberry Pi 3 Model B Rev 1.2
- MainSail OS (from the raspberry pi imager tool)

# About

This should not be considered a plug'n'play config, it is still a work in progress


### What has been configured:
- the X/Y/Z axis, direction, homing, travel direction and dimensions verified 
- The bed and nozzle heat up
- Extruder rotation_distance tuned to my specific printer, a more "default" value is also suggested
- All fans are configured
- filament sensor is configured 
- Config file contains some comments to explain some parts 

### What has not been configured:
- PID tuning, 
  - the pid values are straight from official the I3 config
  - the I3 contains the same mainboard and hot-end 
  - the I3 however has a much smaller printer bed then the chiron, the printer bed doesn't take very long to heat up and I only use the chiron for long prints, so I don't really care 
 - The built-in bed probe has not been configured at all, I havent even mapped out the pins for it. I plan on adding a bltouch to my chiron, so I don't think I will bother with configuring the built-in probe, if you do so, feel free to raise an issue and I will add it to this config 


# Can't flash the mainboard ? 

If you are unable to flash the klipper firmware to your anycubic chiron, you might need to [setup a bootloader for the mainboard](https://github.com/gbit-is/Trigorilla-v0.0.2-burn-bootloader)
