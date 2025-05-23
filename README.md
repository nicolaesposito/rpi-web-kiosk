# rpi-web-kiosk

Complete tutorial on how to build a custom image that turns a Raspberry Pi into a Kiosk serving a web application running in a caged chromium browser instance!

This has been tested on both ARM64 Mac and AMD64 Mac laptops.

AMD is much slower as expected due to emulation.

## Clone the repo

```sh
git clone https://github.com/jonnymacs/rpi-web-kiosk
cd rpi-web-kiosk
```

### kiosk_homepage_url

Set the kiosk_homepage_url in `custom-rpi-image/ext_dir/custom-rpi-image.options`

### device type

Default is Pi5. The img has been tested on Pi4 and Pi5.

If you are on a Pi4, set the device class to pi4 in `custom-rpi-image/ext_dir/config/custom-rpi-image.cfg` 

```
[device]
class=pi4
```

## Build the img

```sh
./build.sh
```

## Write the img to an SD card or USB stick

Use the Raspberry Pi Imager tool to install the img file located in custom-rpi-image/deploy
on an SD card or USB stick

**[Watch and Like the recorded video for this project on YouTube](https://www.youtube.com/watch?v=RnehTqAVqQQ)** 

[![Watch and Like the recorded video for this project on YouTube](https://img.youtube.com/vi/RnehTqAVqQQ/maxresdefault.jpg)](https://www.youtube.com/watch?v=RnehTqAVqQQ)

**[Subscribe to the channel for more similar content](https://www.youtube.com/@macmind-io?sub_confirmation=1)

Please refer to https://github.com/raspberrypi/rpi-image-gen for more information rpi-image-gen

[Follow me on X](https://x.com/jonnymacs), and don't forget to star [this GitHub repository](https://github.com/jonnymacs/rpi-tutorials)!
