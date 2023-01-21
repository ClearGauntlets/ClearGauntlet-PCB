# ClearGauntlet-PCB
PCB - Schematics Design for VR Gloves

A breakout board for ClearGauntlets, aimed at improving cable management and minifying electronics of VR Gloves.

The design consists of two custom PCBs stacked on top of each other, and then an ESP32 on top of that (A "Toast" design).

| Top | Bottom |
|------|-----|
| ![Top PCB CAD Model](https://user-images.githubusercontent.com/42927786/213870192-0c83b508-0c16-4860-ba14-e0bf6b0b3c2c.png) | ![Bottom PCB CAD Model](https://user-images.githubusercontent.com/42927786/213870114-c0028989-27c4-4e96-9cf2-4754b6312ba3.png) |

![Fully assembled](https://user-images.githubusercontent.com/42927786/213871232-e8f9c547-1696-4b3a-904e-89bab2069f54.jpg)

## Specs
The board has two rows of breakout pins that go to finger modules on the glove. Each set of three is Ground, Signal, and Power, of either 3.3v or 5v.

To assemble the board, you'll need
- 41 pins Female Dupont Connectors, 2.54mm pitch (2x 15-pin, 1x 6-pin, 1x 5-pin)
- 13 pins Male Dupont Connectors, 2.54mm pitch (1x 6-pin, 1x 5-pin)
- 46 pins 90° Male Dupont Connectors, 2.54mm pitch (1x 21-pin, 1x 25-pin)
- 1 ESP32

It's all just through-hole soldering, so it goes pretty quick once you have the parts. Use the CAD renders as a guide.

You will also probably want to create a 2-pin 5V USB cable like this one:

![IMG_1019](https://user-images.githubusercontent.com/42927786/213874292-f878529d-52b0-481f-8072-50417f089595.jpg)

It's just power, and ground, and goes into the 5V/GND dupont connector next to the ESP32.

**You'll also need to bodge that 5V in pin to the Vin pin that goes to the ESP32**
