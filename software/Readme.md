
# Pilkki Software
This folder contains the utility to interact with the flasher.

## How to Use

To run the flashing tool:
- Use `cargo run` to run the tool.
- Use `cargo build --release` to build the release version.

The utility should automatically detect the connected port; otherwise, you can specify it manually with the `--port` flag.

### Getting help
```sh
cargo run -- help
```

### Finding the Port to Which Your Device Is Connected:

**Linux:**
```sh
ls /dev/ttyUSB*
```

**MacOS:**
```sh    
ls /dev/tty.* /dev/cu.*
```

### Verify Connection to the Device

To connect to the device, run:
```sh
cargo run -- --port /port/address connect
```

### Flash a New Binary:

To flash a new binary to the device:
```sh
cargo run -- write --input /path/to/your/binary.bin
```
Or, if you need to specify the port manually:
```sh
cargo run -- write --port /port/address --input /path/to/your/binary.bin
```

### Getting the Firmware Binary

You can either:
- Build the binary using the code from the [kampela-firmware](https://github.com/Kalapaja/kampela-firmware) repository.
- Download the compiled binary from the [releases](https://github.com/Kalapaja/kampela-firmware/releases) section.
