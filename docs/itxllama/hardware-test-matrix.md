# ITX Llama Hardware Configuration Tests

## WIP: This page is intended to validate which hardware configurations have been tested to work on the ITX Llama. As test cases are added, their status and any known issues will be noted.

## Storage
| Test             | Status  | Parts Required               | Notes                                     |
| :--------------- | :-----: | :--------------------------- | :---------------------------------------- |
| USB GoTek Floppy | no      | 34pin to USB adapter, GoTek  | BIOS does not recognize USB Floppy drives |
| USB ZuluIDE      | YES     | IDE to USB adapter, ZuluIDE  | ZuluIDE needs FW v2025.01.20, USB adapter needs an "Innostor" bridge chip |
| ZuluIDE (SATA)   | YES     | IDE to SATA adapter, ZuluIDE | ZuluIDE needs FW v2025.01.20, CableCC IDE to SATA adapters work well |
| SATA SSD         | YES     | SATA SSD                     | Just works.                               |
| USB CD-ROM       | YES     | USB CD-ROM                   | Supported, bootable with Linux, DOS not bootable |
| GamePort         | Limited | 2-axis, 2-button controller  | The GamePort on Rev. F shares pins with the S/PDIF output which limits functionality to 2-axis, 2-button controllers. Observed some issues with calibration in Windows 98 |
| 
...more to come.
