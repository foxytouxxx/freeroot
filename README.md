# Foxytoux Installer

## Overview

This shell script is designed to automate the installation of Foxytoux, a lightweight Ubuntu environment using Proot. Foxytoux allows you to run Ubuntu on various CPU architectures, currently supporting x86_64 (amd64) and aarch64 (arm64).

## Prerequisites

- Bash shell environment
- Internet connectivity
- Supported CPU architecture: x86_64 (amd64) or aarch64 (arm64)

## Installation

1. Clone the repository:

    ```sh
    git clone https://github.com/foxytouxxx/freeroot.git
    cd freeroot
    ```

2. Run the installer script:

    ```sh
    ./foxytoux-installer.sh
    ```

3. Follow the prompts to install Foxytoux and, optionally, Ubuntu.

## Supported Architectures

- x86_64 (amd64)
- aarch64 (arm64)

## Usage

After a successful installation, you can run the Foxytoux environment using:

```sh
/path/to/foxytoux-rootfs/usr/local/bin/proot \
  --rootfs="/path/to/foxytoux-rootfs" \
  -0 -w "/root" -b /dev -b /sys -b /proc -b /etc/resolv.conf --kill-on-exit
```

Replace `/path/to/foxytoux-rootfs` with the actual path to your Foxytoux installation.

## License

This Foxytoux Installer script is released under the [MIT License](LICENSE).

## Credits

Foxytoux Installer is developed and maintained by RecodeStudios.Cloud.
This installer has been made possible thanks to [dxomg](https://github.com/dxomg) for his proot code

---

**Note:** This script is intended for educational and experimental purposes. Use it responsibly and at your own risk.
