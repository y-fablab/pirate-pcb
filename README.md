# pirate-pcb

PCB for Pirate Box

![Preview](./doc/preview-3d.jpeg)

## Documentation

* [Schematics](./doc/schematics.pdf)
* [2D Preview](./doc/preview-2d.jpeg)

## Warnings

The WEMOS/LOLIN D1 mini is directly powered by the battery. We typically use 4 AA batteries. Therefore, the power voltage is 6V instead of the 5V usually required. This does not cause any problem, provided that:

1. On the D1 mini, this voltage only powers the 3.3V regulator. This is the case for classic versions of D1 mini where both the CH340 and the SPI memory are powered by 3.3V.
2. When powered through USB, the power goes through a diode. This is the case for all D1 mini versions up to 3.x.x. However, on version 4.0.0, there is no diode and the 6V battery would be connected directly to the USB 5V line, which is not good. Do not use D1 mini version 4.0.0+ on this board.

We recommend using D1 mini v3.x.x and verifying that it has a CH340 chip.

## License

Copyright (c) 2023 [y-fablab.ch](https://www.y-fablab.ch)

Licensed under the [Creative Commons CC-BY 4.0 License](https://creativecommons.org/licenses/by/4.0/)