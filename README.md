# Synth Controller

(forked from [Organelle Controller](https://github.com/critterandguitari/Organelle_Controller))  

MCU firmware.  Interfaces with keys, led, oled, knobs.  Communicates with host via serial OSC.

## Getting Started

(Tested on MacOS)

* Requirements:
  * Make
  * ARM bare-metal toolchain 
    * [Download toolchain](https://developer.arm.com/downloads/-/arm-gnu-toolchain-downloads)
    * Run installer
    * Make sure toolchain is on PATH
  
* Build artifacts
  
  ```bash
  make
  ```

Should see the following output on successful build:

```bash
  text    data     bss     dec     hex filename
  29604     116    3732   33452    82ac build/synth.elf
  arm-none-eabi-objcopy -O ihex build/synth.elf build/synth.hex
  arm-none-eabi-objcopy -O binary -S build/synth.elf build/synth.bin
```
