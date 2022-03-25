# Gantry mounted magprobe for Voron Switchwire conversion (beta)
_This is a beta test, CAD files will be released when the testing phase ends._ \
\
:heavy_exclamation_mark: **if you have a stock Switchwire go to >** [Magprobe for stock Voron Switchwire](https://github.com/salveoo/voronmods/blob/main/Switchwire%20Magprobe/readme.md#magprobe-for-stock-voron-switchwire-beta)

This mod allows you to use a mechanical switch as a probe on your Switchwire conversion without losing any print volume. This remix also negates the need for a dedicated Z-endstop by moving the probe dock to the gantry. \
_This mod was created remixing three mods: \
 • [Klicky](https://github.com/jlas1/Klicky-Probe) \
 • [SideSwipe](https://github.com/oldfar-t/Side-Swipe-Magnetic-Probe) \
 • [Switchwire Magprobe](https://github.com/salveoo/voronmods/tree/main/Switchwire%20Magprobe)_
 
<!---
<p align="center">
  <img width="750" src="https://user-images.githubusercontent.com/44800440/152563247-93c3d950-142e-4bd2-89d5-88d2306ed020.jpg">
</p>
--->

## BOM

#### Motion
* 1x SG90 9g servo

#### Probe
* 1x mouse switch (eg. Omron D2F-5)

#### Fasteners
TBD

#### Magnets
* 5x 6mmx3mm magnets (tested working with N45 magnets)

## Assembly

### Servo bracket assembly
WIP

### Probe assembly

[![Assembly Video](https://user-images.githubusercontent.com/44800440/149659009-e6c0bcc2-035e-4733-a51d-71897badaee7.PNG)](https://youtu.be/O1bFm4f67_E?t=41 "YouTube")

After assembling the probe, check continuity with a multimeter. Follow this from Sideswipe's Github if you have continuity issues: [Probe troubleshooting](https://github.com/oldfar-t/Side-Swipe-Magnetic-Probe#troubleshooting)

### Carriage mount assembly
The carriage mount is remixed from Klicky mod mount. Use 22-24 awg wires.
<p align="center">
  <img width="450" src="https://user-images.githubusercontent.com/44800440/149658491-2cd745b7-0204-4ea6-b79d-f4a45913c59a.PNG">
</p>

Make sure you have enought copper exposed to make good contact
<p align="center">
  <img width="450" src="https://user-images.githubusercontent.com/44800440/149658600-6b11f98c-69b1-4c8f-90c0-92baa65341c1.PNG">
</p>

Insert magnets, then test continuity with a multimeter. Use 2x m3x12mm to bolt it on the carriage.
<p align="center">
  <img width="450" src="https://user-images.githubusercontent.com/44800440/149658667-55900f83-0ddf-436d-b72d-f05ef15fb426.PNG">
</p>

## Macros
I was able to use the incredible klicky probe macros with a small number of tweaks. I simply needed to modify the math in the attach and dock probe macros as well as add the servo in and servo out macros where appropriate. The rest was turn and works great including probe detection and other safety features and checks.
