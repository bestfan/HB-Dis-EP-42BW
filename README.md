# HB-Dis-EP-42BW
### Support for STM32 and RP2040 microcontroller

Inspired by the project of [jp112sdl](https://github.com/jp112sdl/HB-Dis-EP-42BW) I enhanced his solution by the following features:
- Use for STM32 and RP2040 microcontroller (only for mains version)
- Use of other e-paper displays, e.g. 1.54 inch
- Variable number of rows, i.e. lower or equal 10
- Use of GxEPD2 library instead of GxEPD (necessary for RP2040)

When I started this project I just wanted to replace the AT1284 by the RP2040. For testing purpose I used in the beginning a 1.54 inch e-paper display and an STM32 microcontroller. Later on, I came across the application just as an display for remote sensors, e.g. like temperature sensors of fridge and freezer where I was able to use the PCB of my previous project [HB-UNI-Sen-CO2-STM32](https://github.com/bestfan/HB-UNI-Sen-CO2-STM32).

![Display casing](https://github.com/bestfan/HB-Dis-EP-42BW/blob/main/Pictures/display_mod.jpg)

Due to time contraints I have not been able to progress further with a PCB board and a casing for the 4.2 inch display, but I wanted to document at least the completion of the programming and testing.

![Display casing](https://github.com/bestfan/HB-Dis-EP-42BW/blob/main/Pictures/rp2040_mod.jpg)

## Software

### CCU Addon

Please, use the [Addon](https://github.com/jp112sdl/JP-HB-Devices-addon) of the original project. Due to the higher power consumption and the missing battery support the application if restricted to the mains version (RF-type 0xf353)

### Sketch

In comparison to the original work the following libraries is required
- GxEPD2

## Credits

Many thanks to [jp112sdl](https://github.com/jp112sdl/HB-Dis-EP-42BW) for original idea and the many other projects. 

## Disclaimer

The usage of the published software and information is at your own risk and without any warranty.

## License

**Creative Commons BY-NC-SA**<br>
Give Credit, NonCommercial, ShareAlike

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/by-nc-sa.eu.svg" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.
