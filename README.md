# Lab 0 Group E
Status Badge: ![Lab 0 Status](https://github.com/uofu-adv-emb-25/Lab0_GroupE/actions/workflows/main.yml/badge.svg)

Blink code for Pi Pico. Made from the [template repository](https://github.com/uofu-embed/rtos.template) with a modified blink time.
Expects the following environment variables to be set:

    - PICO_SDK_PATH
    - FREERTOS_PATH
    - UNITY_PATH

Clone the appropriate repository and set the variable to the root of the cloned repository.

## Renode setup
The Raspberry Pico needs configuration files for Renode to work properly.

* On MacOS, the installation location is `/Applications/Renode.app/Contents/MacOs`
* On Linux, the location for Debian, Fedora, and Arch is `/opt/renode`
* On Windows, the location is `C://Program Files/Renode`

To add the Pico configuration files:
1. Copy `rp2040_spinlock.py` and `rp2040_divider.py` to the `scripts/pydev` directory of your Renode installation.
1. Copy `rpi_pico_rp2040_w.repl` to the `platforms/cpus` directory.
