# ITX-Llama - Hardware Compatibility Matrix

## Graphics
| Family | Model         | Tested (y/n) | Notes                         |
| :----: | :-----------: | :----------: | :---------------------------- |
| ATI    | Radeon 7500   | y            | Works natively in DOS / Win98 |
| ATI    | Radeon 9250   | y            | Works natively in DOS / Win98 |
| 3DFx   | Voodoo 3      | y            | Works natively in DOS / Win98 |
| 3DFx   | Voodoo 5 5500 | y            | Works natively in DOS / Win98 |
| nVidia | Riva 128      | y            | Works natively in DOS only    |
| nVidia | TNT           | y            | Works natively in DOS only    |
| nVidia | TNT2          | y            | Works natively in DOS only    |
| S3     | Savage4       | y            | Works natively in DOS only    |
| Matrox | G100          | y            | Works natively in DOS only    |

## Wavetable Options
| Module    | MIDI Type                        | Connector   | Notes                                       |
| :----:    | :------------------------------: | :---------: | :------------------------------------------ |
| X2GS      | GM/GS Wavetable                  | Wavetable   | Fits without issue                          |
| **X8GS**  | GM/GS Wavetable                  | Wavetable   | Fits without issue, exclusive to ITX Llama  |
| X16GS     | GM/GS Wavetable                  | Wavetable   | Fits but overlaps Pi headers                |
| OPL-3     | FM Synth                         | OPL Header  | Fits without issue                          |
| Pi Zero 2 | MT-32 / Sound Font               | GPIO Header | Fits without issue                          |
| Pi 4      | MT-32 / Sound Font / Nuked SC-55 | GPIO Header | Fits when attached to a 40pin cable         |
