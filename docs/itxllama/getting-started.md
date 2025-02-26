# Getting Started with your ITX-Llama

Congratulations! You have chosen an excellent modern platform for experiencing many classic MS-DOS and early Windows 98 Games and software. The following guide will help you get started with setting up your ITX-Llama for the first time. 

## Unbox and Assembly

Each ITX-Llama shipped from [Retrodreams.ca](https://retrodreams.ca/collections/all) should come with the following items installed:

* Vortex86EX System-on-Module (CPU, RAM, L1/L2 Cache for your Llama)
* Modem: Wemos D1 Mini ESP8266 for "modem-over-WiFi"

Optionally, you may have elected to include the following items:

* Raspberry Pi Zero 2 w/mt32pi installed
* Dreamblaster X8GS Wavetable MIDI board

### Jumper Configuration
The board should come preinstalled with all the jumpers necessary.  
For changing the configuration, here's a quick walkthrough of the different jumpers and their functionality.

#### PS/2 or USB HID
Jumpers: `J7`, `J12`, `J15`, `J16`
<p>
  <img src=../images/usb-ps2.jpg title="PS/2 configuration" width=35%>
</p>

* If you want to use a real PS/2 keyboard connected to the purple PS/2 port, place the two top-most jumpers (`J15` and `J16`) to the leftmost position ("PS/2"). For USB HID keyboard connected to one of the white USB ports (between the PS/2 and serial port), place the jumpers to the rightmost side ("USB").
* If you want to use a real PS/2 mouse connected to the green PS/2 port, place the two bottom-most jumpers (`J7` and `J12`) to the left-most position ("PS/2"). For USB HID mouse connected to one of the white USB ports (between the PS/2 and serial port), place the jumpers to the rightmost side ("USB").

#### Line In
Jumpers: `J39`, `J40`
<p>
  <img src=../images/line-in.jpg title="Line In" width=35%>
</p>

* If you want to use an external audio source connected to the blue 3.5mm jack port, place both jumpers to the leftmost position ("EXT").  
* To Select a Raspberry Pi Zero2 or Wavetable board as line-in to the sound card, place the two jumpers to the rightmost position ("INT").

#### Pi or Wavetable

Jumpers: `J26`, `J27` <br>
_Note: Batch 2 - Rev F boards removed the Power jumper `J25`_
<p>
  <img src=../images/pi-wt.jpg title="PI/WT configuration" width=35%>
</p>

* To Select a Raspberry Pi (Zero2, 3 or 4) for converting MIDI to analog audio, place the two jumpers to the rightmost position ("PI").  
* To Select a Wavetable board, place the jumpers to the leftmost position ("WT").

#### Fans
The Vortex86EX SOM doesn't draw much power, and shouldn't require active cooling if running at or below 300 MHz.  
If you do wish to add one or more fans, the motherboard has three separately controllable 4-pin PWM fan connectors:
<p>
  <img src=../images/fan-1.jpg title="Fan header" width=35%>
</p>
Simply connect a modern 4-pin fan to one of these headers, and set the corresponding jumper to either 5V or 12V:
<p>
  <img src=../images/fan-2.jpg title="Fan configuration" width=35%>
</p>

Note: Take care **not** to supply 12V to a 5V fan - you'll likely fry it.

## Setup and Installation

### MS-DOS Installation

TODO: Fill this out

### Windows 98 Installation

TODO: Fill this out


[winworldpc-win98]: https://winworldpc.com/download/417d71c2-ae18-c39a-11c3-a4e284a2c3a5
[vogons-thread]: https://www.vogons.org/viewtopic.php?t=93480
[mt32-pi]: https://github.com/dwhinham/mt32-pi
[mt32-pi-control]: https://github.com/gmcn42/mt32-pi-control/tree/main/dos_bin