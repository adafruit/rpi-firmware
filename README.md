adafruit rpi-firmware

Raspberry Pi kernel 3.15.8+, with additional patches for Adafruit devices
such as LCDs (via fbtft).

Based heavily on rpi-firmware from notro: https://github.com/notro/rpi-firmware

Install
-------

Get rpi-update from https://github.com/Hexxeh/rpi-update

```text
sudo REPO_URI=https://github.com/adafruit/rpi-firmware rpi-update
```

Kernel Source
-------------

* https://github.com/adafruit/adafruit-raspberrypi-linux

The fbtft repo is a submodule of adafruit-raspberrypi-linux.  You can fetch
it as part of the clone by running:

    git clone --recursive https://github.com/adafruit/adafruit-raspberrypi-linux.git

It is, however, available separately at:

* https://github.com/adafruit/adafruit-rpi-fbtft.git

Kernel Config
-------------

The kernel config file is found in the adafruit rpi kernel.  You can activate
it by checking out 3.15.8+ and running

    make adafruit_defconfig
