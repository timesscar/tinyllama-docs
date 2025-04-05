# Getting Started with your ITX-Llama - Setting up DOS

The following guide will help you get started with setting up DOS on your ITX-Llama. 

---

### MS-DOS Installation

1. Choose your favorite VFD (Virtual Floppy Disc) in BIOS
1. Insert a blank SD card (128GB or less is ideal), or SATA SSD
1. Ensure you're booting from your chosen VFD by pressing `ESC` during start-up and selecting the Virtual Floppy image.
1. Format your chosen fixed storage device as normal. See example below: 
    * From the A: drive, run `fdisk c:` _follow the prompts._ 
      * Note: MS-DOS 6.22 is restricted to FAT16 out of the box and thus up to 4, 2GB partitions.
    * From the A: drive, run `format c: /s` _follow the prompts._
    * From the A: drive, run `copy *.* c:`
    * Adjust any file references in `autoexec.bat` / `config.sys`.
    * From the C: drive, run `fdisk /mbr` to ensure your C: drive is bootable.
    * Reboot.
1. As an alternative, the MiNiDOS VFD offers an install process which automates most of these steps.

---

### FreeDOS SD Card Image (pre-loaded)
1. Purchase an SD card from [Retrodreams.ca][Retrodreams-FreeDOS] preloaded with FreeDOS.
2. Check out this [README](freedos-sdcard.md)
3. Insert the SD Card into your ITX-Llama and enjoy!

---

### DOS Drivers
* [DOS Drivers](setup.md#dos-drivers)

---

[Back to Setup](setup.md) <br>
[Back to Getting Started](../getting-started.md)


[itxllama-repo]: https://github.com/eivindbohler/itxllama/archive/refs/heads/main.zip
[Retrodreams]: https://retrodreams.ca/collections/all
[Retrodreams-FreeDOS]: https://retrodreams.ca/products/preloaded-microsd-card-with-freedos-goodies
[winworldpc-win98]: https://winworldpc.com/download/417d71c2-ae18-c39a-11c3-a4e284a2c3a5
[vogons-thread]: https://www.vogons.org/viewtopic.php?t=93480
[vogons-minidos]: https://www.vogons.org/viewtopic.php?p=1307896#p1307896
[mt32-pi]: https://github.com/dwhinham/mt32-pi
[mt32-pi-control]: https://github.com/gmcn42/mt32-pi-control/tree/main/dos_bin