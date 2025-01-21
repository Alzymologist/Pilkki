
# Pilkki
SWD flashing tool for EFM32 microcontrollers.

## Project structure

The project is divided into three parts:

1. **[Software](software)**: The flashing utility.
2. **[Electronics](electronics)**: Schematics and PCB (KiCAD).
3. **[Firmware](firmware)**: Firmware for the target device.

### How to Use

To use the flasher, you can either:

- Run the utility directly with `cargo run`
- Build the project in release mode with `cargo build --release`

More info on how to use pilkki in [Readme.md](software/Readme.md) in the [Software](software) section