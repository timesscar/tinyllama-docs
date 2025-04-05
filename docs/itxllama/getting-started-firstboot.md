# Getting Started with your ITX-Llama

The following guide will give you a quick tour of a few BIOS settings to get you started. 

## First Boot Tour

Your ITX Llama should have shipped with `ITX-Llama v1-rev-F - 20250302-063713`. <br>
Beginning with this revision, here are a few features to help you get started.

### Boot Device Order defaults to "SD card, SATA, USB, VFD (Virtual Floppy Disc)"

* _(You can override this order by pressing `ESC` during the Energy Star Logo)_
* <p>
    <img src=../images/bios-settings-disks-bootorder.png title="BIOS Settings - Boot Order" width=50%>
  </p>

---

> ### USB as Fixed Disks Quirk

  * The "USB as Fixed Disks" feature is known to cause issues in Windows 98. Set "USB as Fixed Disks" to "Disabled" if you encounter difficulties with slowdowns, corrupt disks or graphical glitches. This means that Windows will need separate USB driver support to read/write from USB drives.
  * <p>
    <img src=../images/bios-settings-disks.png title="BIOS Settings - Boot Order" width=50%>
  </p>

---

## Selecting a Virtual Floppy Disk (VFD)

<p>
    <img src=../images/bios-settings-disks-vfds.png title="BIOS Settings - Boot Order" width=50%>
</p>

### VFD: "**MS-DOS 6.22**" (default)

* This virtual floppy image is embedded in the system BIOS and contains many tools to help get you started with building an MS-DOS 6.22 system.
* On this virtual disk, you will find drivers for a PS/2+Serial mouse, USB CD drivers, SATA CD Drivers and memory management tools designed to work with MS-DOS 6.22.
* <p>
    <img src=../images/vfd-msdos-622.png title="MS-DOS 6.22 VFD" width=35%>
  </p>

### VFD: "**Windows 98 (DOS 7.1)**"

* This virtual floppy image is embedded in the system BIOS and contains many tools to help get you started building a Windows 98 and/or DOS 7.1 system.
* On this virtual disk, you will find drivers for a PS/2+Serial mouse, USB CD drivers, SATA CD Drivers and memory management tools designed to work with MS-DOS 7.1.
* <p>
    <img src=../images/vfd-windows-98.png title="Windows 98 VFD" width=35%>
  </p>

### VFD: "**MiNiDOS 2025 v0.02.1**"

* This virtual floppy image is embedded in the system BIOS a highly customized MS-DOS 6.22 single disc installer. <br>
    **Shout-out to MiNiDOS on VOGONs!** [-thread here-][vogons-minidos]
* On this virtual disk, you will find a single-disc installer for MS-DOS 6.22 assembled by MiNiDOS on VOGONS. Additionally, this image was slightly customized for the IXT-Llama to include drivers for USB and SATA CD Drives.

[Back to Getting Started](getting-started.md)

[Retrodreams]: https://retrodreams.ca/collections/all
[winworldpc-win98]: https://winworldpc.com/download/417d71c2-ae18-c39a-11c3-a4e284a2c3a5
[vogons-thread]: https://www.vogons.org/viewtopic.php?t=93480
[vogons-minidos]: https://www.vogons.org/viewtopic.php?p=1307896#p1307896
[mt32-pi]: https://github.com/dwhinham/mt32-pi
[mt32-pi-control]: https://github.com/gmcn42/mt32-pi-control/tree/main/dos_bin