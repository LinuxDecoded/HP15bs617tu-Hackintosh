# Hp 15bs617tu Opencore EFI MacOS Monterey
![Hp Latpop Image](/Docs/myHP.png)





### Currently Running:


| Component     | Version         |
| ------------- | --------------- |
| macOS version | 12.0.1 (21A559) |
| OpenCore      | 0.7.5           |

## Hardware Info

| Component | Model                                   |
| --------- | --------------------------------------- |
| CPU                           | Intel® Core™ i3-6006U (2 GHz, 3 MB cache, 2 cores)                    |
| Memory                        | 4 GB DDR4-2133 SDRAM (1 x 4 GB)                                       |
| Storage                       | Toshiba 1 TB 5400 rpm SATA                                            |
| Display                       | 39.62 cm(15.6) diagonal FHD (1920 x 1080)                             |
| GPU [`iGPU`]                  | Intel HD 520                                                          |
| Camera                        | HP TrueVision HD Camera with integrated digital microphone            |
| WLAN                          | Realtek RTL8723DE 802.11b/g/n (1x1) and Bluetooth® 4.0 combo          |
| Touchpad                      | Synaptics PS2 Touchpad with multi-touch gesture support               |
| Battery Type                  | 4-cell, 41 Wh Li-ion                                                  |

## Kexts

| Kext                   | Version     | Remark                                   |
| ---------------------- | ----------- | ---------------------------------------- |
| AppleALC               | 1.6.5       | Fixes onboard audio                      |
| Lilu                   | 1.5.6       | Kext patcher                             |
| ACPIBatteryManager     | 1.2.4       | Battery indicator                        |
| SMCProcessor           | 1.2.7       | CPU temp monitoring                      |
| SMCSuperIO             | 1.2.7       | Monitor fan speed, not working           |
| VirtualSMC             | 1.2.7       | SMC chip emulation                       |
| VoodooPS2Controller    | 2.2.6       | PS2 driver                               |
| WhateverGreen          | 1.5.4       | Graphics                                 |
| RealtekRTL8111         | 2.4.2       | Ethernet                                 |
| BrightnessKeys         | 1.0.2       | Fixes Brighness function keys            | 
| ECEnabler              |

## ACPI patches

All of the following SSDT's have been manually compiled by me such that they improve performance and boot time. *These will not work for other laptops.*

| Patch                 | Remark                         |
| --------------------- | ------------------------------ |
| SSDT-PLUG             | x86 plugin injection fix       |
| SSDT-PNLF             | Backlight fix                  |
| SSDT-EC-USBX          | USBX patch                     |
| SSDT-RTC0             | RTC patch (Super necessary to boot this specific model) |
| SSDT-SBUS-MCHC        | Fixing SMBus support           |
## Status

### Working

- [x] Keyboard (including all media keys and brightness keys)
- [x] Battery indicator
- [x] Audio
- [x] Ethernet
- [x] iCloud services - iMessage, FaceTime, AppStore
- [x] GPU acceleration
- [x] Camera
- [x] Microphone
- [x] Mac-like booting interface for multiboot
- [x] Sleep/wake
- [x] Trackpad and gestures



### Not Working at the moment
- [ ] Wifi
- [ ] Bluetooth
- [ ] Display auto brightness
- [ ] Handoff, continuity
- [ ] AirPlay

### Not Tested

- [ ] Sidecar
- [ ] FileVault
- [ ] DRM content playback (Netflix, Apple TV+)
- [ ] HDMI

For Networking with USB WIFI Dongle use this driver -- 
(https://github.com/chris1111/Wireless-USB-OC-Big-Sur-Adapter)


## This OpenCore EFI is full-fleged, I haven't removed a single thing from it  Even the OpenCore boot menu is GUI with mouse support

## CREDITS

- [Acidanthera](https://github.com/acidanthera)
- [Dortania OC guide](https://dortania.github.io/OpenCore-Install-Guide/)

 
