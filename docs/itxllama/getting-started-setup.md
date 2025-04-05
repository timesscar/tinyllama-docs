# Getting Started with your ITX-Llama

The following set of guides aim to help you set up an operating system on your ITX-Llama. 

---

### MS-DOS Installation

See [MS-DOS Setup Guide](getting-started-setup-dos.md)

---

### Windows 98 Installation

See [Windows 98 Setup Guide](getting-started-setup-win98.md)

---

### FreeDOS SD Card Image (pre-loaded)
1. Purchase an SD card from [Retrodreams.ca][Retrodreams-FreeDOS] preloaded with FreeDOS.
2. Check out this [README](getting-started-freedos-sdcard.md)
3. Insert the SD Card into your ITX-Llama and enjoy!

---

### DOS Drivers

* [ctmouse.exe][driver-CTMOUSE] - The venerable FreeDOS Mouse Driver - CTMouse! (v2.1b)
* [pmouse.com][driver-PMOUSE] - A smaller, lighter sometimes more compatible alternative to CTMouse

### Windows 98 Drivers

* [Crystal 4237b v2.86][driver-win98-CWD] - Windows 98 drivers tuned for the Llama's Crystal 4237b sound chip.
* [Realtek R6040 10/100 NIC][driver-win98-R6040] - Windows 98 drivers for the integrated Vortex86EX network interface.
* [Large Drive Support (tbplus) Patch][driver-win98-TBPLUS] - Windows 98 Patch for Large HDD support. (subset of TBPlus Pack)
* [USB Removable Storage Driver][driver-win98-USB] - Windows 98 USB removable storage driver (nusb36e)

### Tools

* [cwdmix.exe][tool-CWDMIX] - DOS Utility for setting mixer levels for the Crystal 4237b sound chip.
* [anybios.exe][tool-ANYBIOS] - DOS Utility for flashing the ITX Llama system BIOS.
* [slowdown.zip][tool-SLOWDOWN] - DOS Utility for slowing the CPU down even further than the lowest clock selectable in BIOS.
* [Large Drive Support w/Tools (tbplus)][driver-TBPLUS-Full] - Allows Windows 98SE to use hard drives larger than 1TB. (Full TBPlus Pack including DOS partitioning tools)

[Back to Getting Started](getting-started.md)

[driver-CTMOUSE]: https://docs.retrodreams.ca/itxllama/binaries/DOS-utils/CTMOUSE.EXE
[driver-PMOUSE]: https://docs.retrodreams.ca/itxllama/binaries/DOS-utils/PMOUSE.COM
[tool-CWDMIX]: https://docs.retrodreams.ca/itxllama/binaries/DOS-utils/CWDMIX.EXE
[tool-ANYBIOS]: https://docs.retrodreams.ca/itxllama/binaries/DOS-utils/ANYBIOS.EXE
[tool-SLOWDOWN]: https://docs.retrodreams.ca/itxllama/binaries/DOS-utils/SLOWDOWN.ZIP
[driver-TBPLUS-Full]: https://docs.retrodreams.ca/itxllama/binaries/WIN98-drivers/TBPLUS/TBPLUS_FULL.zip
[driver-win98-TBPLUS]: https://docs.retrodreams.ca/itxllama/binaries/WIN98-drivers/TBPLUS/TBPLUS.zip
[driver-win98-CWD]: https://docs.retrodreams.ca/itxllama/binaries/WIN98-drivers/CWD-v286-1998-itx-llama/CWD_DRVS.zip
[driver-win98-R6040]: https://docs.retrodreams.ca/itxllama/binaries/WIN98-drivers/r6040_win98/r6040_win98.zip
[driver-win98-USB]: https://docs.retrodreams.ca/itxllama/binaries/WIN98-drivers/USB/nusb36e.exe
[os-win98-part1]: https://docs.retrodreams.ca/itxllama/binaries/WIN98/WIN98_1.zip
[os-win98-part2]: https://docs.retrodreams.ca/itxllama/binaries/WIN98/WIN98_2.zip
[os-win98-archive]: https://archive.org/details/win-98-1
[itxllama-repo]: https://github.com/eivindbohler/itxllama/archive/refs/heads/main.zip
[Retrodreams]: https://retrodreams.ca/collections/all
[Retrodreams-FreeDOS]: https://retrodreams.ca/products/preloaded-microsd-card-with-freedos-goodies
[winworldpc-win98]: https://winworldpc.com/download/417d71c2-ae18-c39a-11c3-a4e284a2c3a5
[vogons-thread]: https://www.vogons.org/viewtopic.php?t=93480
[vogons-minidos]: https://www.vogons.org/viewtopic.php?p=1307896#p1307896
[mt32-pi]: https://github.com/dwhinham/mt32-pi
[mt32-pi-control]: https://github.com/gmcn42/mt32-pi-control/tree/main/dos_bin