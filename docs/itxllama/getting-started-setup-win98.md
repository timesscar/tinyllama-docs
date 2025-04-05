# Getting Started with your ITX-Llama - Setting up Windows 98

The following guide will help you get started with setting up Windows 98 on your ITX-Llama. 

### Windows 98 Installation

1. Prepare a Windows 98 CD.
    * This can be an OEM CD or a blank CD filled with **_unzipped_** versions of these files: 
    [Slip-streamed Install Files][os-win98-archive]
    * These Windows 98 installation files contain ITX-Llama specific drivers slip-streamed into the installation.
1. Choose the "Windows 98 (DOS 7.1)" VFD (Virtual Floppy Disc) in BIOS
1. Insert a blank SD card (128GB or less is ideal), or SATA SSD
1. Ensure you're booting from "Windows 98 (DOS 7.1)" VFD by pressing `ESC` during start-up and selecting the Virtual Floppy image.
1. Format your chosen fixed storage device as normal. See [#MS-DOS Installation].
1. Restart your ITX-Llama
1. Ensure you're booting from "Windows 98 (DOS 7.1)" VFD by pressing `ESC` during start-up and selecting the Virtual Floppy image.
1. Select the "Setup Windows 98" option.  _setup should begin._

### Windows 98 Installation to SATA Drive
1. Prep SDCard as installer:
    a.  Extract ISO of windows 98 SE to root of SDCard
    b.  Download copy of [this repository][itxllama-repo] and extract the ZIP file, place the folder itxllama-main onto the SDCard
    c.  Place SDCard into ITX Llama
1. Boot ITX Llama, change BIOS settings so SATA drive is first priority (F1 to enter BIOS)
1. Under Disk Settings, (use the left and right arrow keys to switch between panes) set :
    a.  Boot Order to anything with SATA first. 
    b.  Virtual Floppy to Windows 98 (DOS 7.1)
    c.  USB as Fixed Disks: Disabled
1. Save settings with `F10`, this will save and reboot the BIOS settings
1. Press `ESC` during boot-up and choose the Win98 Boot Disk
1. Choose option 3 `Start ITX-Llama without CD-ROM Support`
1. Partition the SATA disk using `xfdisk`:
    a.  Follow the instructions onscreen in order to partition the hard disk
    b.  Once complete, reboot the computer and follow steps 5-6 again
1. Once rebooted, try to navigate to the C:, it should give an error saying the disk is not formatted. Press `A` to abort, then go back to the A: and run `format C:`
1. After formatting C:, let’s copy the windows 98 files onto the SATA disk. First, we need to extract xcopy  files from the media, go to the WIN98 folder on the D:, then use the following command `extract /a win98_47.cab xcopy*.*`
1. Create a win98 folder on the C: (this will hold the installation files), `md C:\win98`
1. Copy the files over, `xcopy /a /s *.* C:\win98 `
1. Create a folder on the C: for the itx-llama patches (we will need to use these soon), `md C:\itxdrvs`
1. Copy the files from the itx-llama patches folder to the C:, don’t leave the win98 folder: `xcopy /a/s \itxll~94\win98~19\*.* C:\itxdrvs\` (remember to use tab completion in order to auto-fill the folder names in correctly)
1. Launch `setup.exe` in C:\win98 and complete the installation...
1. The system will reboot from GUI install mode. This is where we need to install the ITX Llama drivers packages. When the system tells you to remove the floppy disks and reboot, during that reboot start pressing F8 to force Windows to bring up the boot menu. 
1. Select `Safe-Mode Command Prompt Only` (Shift + F5)
1. In the command prompt: `cd \itxdrvs` then `install C:\windows`
1. Eject the SDCard, then reboot the system
1. Windows should complete without any issues at this point. 

The author of this section notes there are incompatibilities with the driver `esdi_506.pdr` when Windows 98 is being loaded. This issue is mitigated when the SDCard is removed. -- 03/17/2025 danifunker

[Back to Setup](getting-started-setup.md) <br>
[Back to Getting Started](getting-started.md)

[os-win98-archive]: https://archive.org/details/win-98-1
[itxllama-repo]: https://github.com/eivindbohler/itxllama/archive/refs/heads/main.zip
[Retrodreams]: https://retrodreams.ca/collections/all
[Retrodreams-FreeDOS]: https://retrodreams.ca/products/preloaded-microsd-card-with-freedos-goodies
[winworldpc-win98]: https://winworldpc.com/download/417d71c2-ae18-c39a-11c3-a4e284a2c3a5
[vogons-thread]: https://www.vogons.org/viewtopic.php?t=93480
[vogons-minidos]: https://www.vogons.org/viewtopic.php?p=1307896#p1307896
[mt32-pi]: https://github.com/dwhinham/mt32-pi
[mt32-pi-control]: https://github.com/gmcn42/mt32-pi-control/tree/main/dos_bin