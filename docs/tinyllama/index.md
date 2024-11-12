# TinyLlama Project

The TinyLlama is a modern recreation of the best that late DOS/early Windows 98 computing had to offer, now reimagined into an truly tiny form-factor! For more information, visit the [Vogons thread][vogons-thread].

## Documentation Contents
- [Overview](https://github.com/eivindbohler/tinyllama/blob/main/README.md)

## Specs
- **CPU:** Designed specifically for the Vortex86EX System on Module:
    - High performance, 32bit 486/Pentium equivalent CPU
        - Selectable clock from 60MHz to 500MHz
        - 16KB WT L1 cache
        - 128BK WT/WB L2 Cache
        - [...more information](https://www.vortex86.com/products/Vortex86EX)
- **RAM:** 128MB DDR3
- **Sound:** 
    - Crystal Audio CS4237B for Soundblaster 16 emulation
    - mt32pi for Roland MT-32 emulation

## Connectivity
- USB Micro-B for power (draws ~4.5W with a Pi attached, ~3W without, depending on CPU frequency)
- 2 x USB Type-A 2.0 connectors for keyboard/mouse/storage
- MicroSD slot for storage
- DE-9 RS232 serial port (COM1)
- Internal 3-pin TTL serial connector (COM2)
- Internal 2-pin power connector for a fan (5V or 3.3V selectable)
- 3.5mm line-out audio jack

[vogons-thread]: https://www.vogons.org/viewtopic.php?f=25&t=84880
[mt32-pi]: https://github.com/dwhinham/mt32-pi