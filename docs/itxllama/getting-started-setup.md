# Getting Started with your ITX-Llama

The following guide will help you get started with setting up an operating system on your ITX-Llama for the first time. 

## Setup and Installation

### MS-DOS Installation

1. Choose your favorite VFD (Virtual Floppy Disc) in BIOS
1. Insert a blank SD card (128GB or less is ideal), or SATA SSD
1. Ensure you're booting from your chosen VFD by pressing `ESC` during start-up and selecting the Virtual Floppy image.
1. Format your chosen fixed storage device as normal. See example below: 
    * `A:> fdisk c:` _follow the prompts._ 
      * Note: MS-DOS 6.22 is restricted to FAT16 out of the box and thus up to 4, 2GB partitions.
    * `A:> format c: /s` _follow the prompts._
    * `A:> copy *.* c:` 
    * Adjust any file references in `autoexec.bat` / `config.sys` and reboot.
1. As an alternative, the MiNiDOS VFD offers an install process which automates most of these steps.

### Windows 98 Installation

1. Prepare a Windows 98 CD.
    * This can be an OEM CD or a blank CD filled with **_unzipped_** versions of these files: [win98-p1][os-win98-part1], [win98-p2][os-win98-part2]
    * These Windows 98 installation files contain ITX-Llama specific drivers slip-streamed into the installation.
1. Choose the "Windows 98 (DOS 7.1)" VFD (Virtual Floppy Disc) in BIOS
1. Insert a blank SD card (128GB or less is ideal), or SATA SSD
1. Ensure you're booting from "Windows 98 (DOS 7.1)" VFD by pressing `ESC` during start-up and selecting the Virtual Floppy image.
1. Format your chosen fixed storage device as normal. See [#MS-DOS Installation].
1. Restart your ITX-Llama
1. Ensure you're booting from "Windows 98 (DOS 7.1)" VFD by pressing `ESC` during start-up and selecting the Virtual Floppy image.
1. Select the "Setup Windows 98" option.  _setup should begin._

### FreeDOS SD Card Image (pre-loaded)
1. Purchase an SD card from [Retrodreams.ca][Retrodreams-FreeDOS] preloaded with FreeDOS.
2. Check out this [README](getting-started-freedos-sdcard.md)
3. Insert the SD Card into your ITX-Llama and enjoy!


[driver-CTMOUSE]: https://docs.retrodreams.ca/itxllama/DOS-utils/CTMOUSE.EXE
[driver-CWDMIX]: https://docs.retrodreams.ca/itxllama/DOS-utils/CWDMIX.EXE
[driver-win98-CWD]: https://docs.retrodreams.ca/itxllama/WIN98-drivers/CWD-v286-1998-itx-llama/CWD_DRVS.zip
[driver-win98-R6040]: https://docs.retrodreams.ca/itxllama/WIN98-drivers/r6040_win98/r6040_win98.zip
[os-win98-part1]: https://docs.retrodreams.ca/itxllama/WIN98/WIN98_1.zip
[os-win98-part2]: https://docs.retrodreams.ca/itxllama/WIN98/WIN98_2.zip
[Retrodreams]: https://retrodreams.ca/collections/all
[Retrodreams-FreeDOS]: https://retrodreams.ca/products/preloaded-microsd-card-with-freedos-goodies
[winworldpc-win98]: https://winworldpc.com/download/417d71c2-ae18-c39a-11c3-a4e284a2c3a5
[vogons-thread]: https://www.vogons.org/viewtopic.php?t=93480
[vogons-minidos]: https://www.vogons.org/viewtopic.php?p=1307896#p1307896
[mt32-pi]: https://github.com/dwhinham/mt32-pi
[mt32-pi-control]: https://github.com/gmcn42/mt32-pi-control/tree/main/dos_bin