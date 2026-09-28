# OVERPAD

A custom 12-key mechanical macropad with a rotary encoder, OLED display and RGB, powered by QMK.

<sub>[@lastlxrd](https://github.com/lastlxrd) · 2024</sub>

<p align="center">
  <img src="docs/overpad1.jpg" width="900">
</p>

<p align="center">
  <img src="docs/overpad2.jpg" width="900">
</p>

<p align="center">
  <img src="docs/overpad3.jpg" width="900">
</p>

OVERPAD is a compact programmable macropad built around the ATmega32U4 and QMK Firmware.

## Features

- 12 mechanical keys
- Rotary encoder with push button
- ATmega32U4 microcontroller
- 128×64 OLED display
- 12× WS2812 RGB LEDs
- USB HID
- QMK Firmware
- NKRO support
- Mouse keys and media controls
- Caterina bootloader

## Hardware

| Component | Description |
|---|---|
| MCU | ATmega32U4 |
| Keys | 12 mechanical keys |
| Encoder | Rotary encoder with push button |
| Display | 128×64 OLED |
| RGB | 12× WS2812 LEDs |
| Firmware | QMK |
| Bootloader | Caterina |

## Firmware

The firmware is based on [QMK Firmware](https://qmk.fm/).

The repository contains the keyboard configuration files:

```text
.
├── config.h
├── keyboard.json
├── rules.mk
├── docs/
│   ├── overpad1.jpg
│   ├── overpad2.jpg
│   └── overpad3.jpg
└── README.md
```

To use the keyboard definition inside a QMK installation, place it in:

```text
qmk_firmware/keyboards/lastlxrd/overpad/
```

A QMK keymap can then be placed inside:

```text
keymaps/default/
```

and compiled with:

```bash
qmk compile -kb lastlxrd/overpad -km default
```

or flashed with:

```bash
qmk flash -kb lastlxrd/overpad -km default
```

> A `keymaps/default/keymap.c` file is required to build a complete firmware image.

## About

OVERPAD is an early custom hardware project developed in 2024.

The project combines PCB design, embedded firmware and mechanical keyboard hardware in a compact programmable controller.

## Author

Designed and developed by [lastlxrd](https://github.com/lastlxrd).