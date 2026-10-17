# lineageos-pdx246-releases
Unofficial LineageOS releases for the [Sony Xperia 10 VI (pdx246)](https://www.gsmarena.com/sony_xperia_10_vi-13002.php) [XQ-ES54, XQ-ES72] 

Based on:
* [pdx246 device tree](https://github.com/johanneszab/android_device_sony_pdx246)
* [sm6450 kernel source](https://github.com/johanneszab/android_kernel_sony_sm6450) 
* [sm6450-modules kernel source](https://github.com/johanneszab/android_kernel_sony_sm6450-modules)
* [sm6450-devicetrees](https://github.com/johanneszab/android_kernel_sony_sm6450-devicetrees)
* [LineageOS](https://gitlab.com/LineageOS)

## How to flash

Before flashing, make sure you meet the following requirements:
* A XQ-ES54 or XQ-ES72 variant. I only own the XQ-ES54 myself, but a user reported the XQ-ES72 working: calls work, and it identifies itself as XQ-ES72.
* Your phone is updated to at least any of the 70.2.A.* Sony stock rom versions (e.g. Android 16).
* Flash it like any other LineageOS Sony ROM. Follow, for example the [official lineageOS instruction for the Sony
  Xperia 10 VII](https://wiki.lineageos.org/devices/pdx257/install/), but with the
  [release files for the Sony Xperia 10 VI](https://github.com/johanneszab/lineageos-pdx246-releases/releases).
* If you want to use Google Apps (Gapps), use the MindTheGapps release that matches the LineageOS
  version: [17.0.0-arm64 for LineageOS 24](https://github.com/MindTheGapps/17.0.0-arm64/releases),
  [16.0.0-arm64 for LineageOS 23](https://github.com/MindTheGapps/16.0.0-arm64/releases).
  Sideload them in recovery right after the LineageOS zip, before the first boot.

## Upgrading from LineageOS 23.2 to 24.0

Your data stays. In recovery, sideload the 24.0 zip, accept the offer to install additional
packages, sideload MindTheGapps 17.0.0-arm64 (if you use Gapps), then reboot. Do not boot
Android between the two, or the Google apps end up without their privileges. Details are in
the [24.0 release notes](https://github.com/johanneszab/lineageos-pdx246-releases/releases/tag/v24.0-20261015).
Going back from 24.0 to 23.2 needs *Format data*.
  
