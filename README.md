# Lee's Custom Ergodox Firmware

This is the firmware that I've generated for my [Infinity Ergodox][ergodox] keyboard.

## Requirements

* **MUST** use Dvorak layout as the default layer
* **MUST** move keys important to programming as little as possible - braces, `+`, `-`, `/`, etc
* **MUST** have a shiftable layer for access to media keys - Volume Up, Volume Down, Mute, Play/Pause, Next, and Previous
* **MUST** have a key combination to enable flashing
* **SHOULD** offer a QWERTY layout on a lockable layer

## Installation

:rotating_light: These are my personal notes. [The real instructions][instructions] can be found on the [Input Club website][input-club]. :rotating_light:

### Setup

1. `brew update`
1. `brew install dfu-util`

### Flashing

The keyboard is in two parts that are daisy-chained together. The keyboard side that comes first in the daisy-chain is the primary side. There are two `*.bin` files in the repository, you must flash the `.bin` file that corresponds to the primary side.

1. `dfu-util -D [.bin file]`

## Acknowledgements

* The initial version of this firmware was generated using the awesome [Kiibohd Configurator][configurator]
* Many thanks to Input Club and many others for bringing these awesome kits and tools to life

[configurator]: https://input.club/configurator
[ergodox]: https://input.club/devices/infinity-ergodox
[input-club]: https://input.club/
[instructions]: https://github.com/kiibohd/controller/wiki/Loading-DFU-Firmware
