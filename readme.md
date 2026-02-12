# KBD firmware

## How to build

## 1. Setting Up Your QMK Environment

Please see https://docs.qmk.fm/#/newbs_getting_started and set up 1 to 3.

## 2. Files to Modify

- `keyboards\crkbd\vial-kb\vial-qmk\keymaps\vial\config.h`
- `keyboards\crkbd\vial-kb\vial-qmk\keymaps\vial\keymap.c`
- `keyboards\crkbd\vial-kb\vial-qmk\keymaps\vial\rules.mk`

## 3. Quick Notes for Compiling and Flashing

1. open qmk msys terminal
2. `cd source/kbd_firmware/`
3. `make vial-qmk-clean && kb=crkbd make vial-qmk-init && kb=crkbd kr=rev4_1/standard km=vial make vial-qmk-compile`
4. unplug the keyboard, hold down the top row 2nd to far outside key, plug in that half of the keyboard, a drive mount will popup/appear
5. `kb=crkbd kr=rev4_1/standard km=vial make vial-qmk-flash`
6. repeat 4. and 5. for the other half of the keyboard
