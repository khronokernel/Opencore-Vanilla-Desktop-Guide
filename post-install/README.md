# Post Install

* Supported version: 0.5.7

**Attention to all users, please note this guide and other khronokernel sites will be shutting down on April 16th, 2020. Reason for this is we've decided to move the guides to a dedicated organization to help simplify the hackintosh process and provide a single, trusted source for hackintosh information. This new organization will be known as [Dortania](https://github.com/dortania).**

Links to the new sites:

* [OpenCore Desktop Guide](https://desktop.dortania.ml/)
* [Getting Started with ACPI](https://acpi.dortania.ml/)
* [GPU Buyers Guide](https://gpu.dortania.ml/)
* [Wireless Buyers Guide](https://wifi.dortania.ml/)
* [Anti-Hackintosh Buyers Guide](https://hardware.dortania.ml/)

So you've finally finsihed installing macOS with OpenCore but know there's still some things to clean up, well you've come to the right place!

## Universal

This section is benificial for all, regardless of hardware.

* [Correcting Audio](/post-install/audio.md)
* [Enabling FileVault and other security features](/post-install/security.md)
* [Booting macOS without a USB](/post-install/oc2hdd.md)
* [Updating OpenCore, kexts and macOS](/post-install/update.md)
* [Disabling OpenCore Logging](/troubleshooting/debug.md)
* [Fixing iServices](/post-install/iservices.md)
* [Fixing DRM](/post-install/drm.md)

## Intel

Used for Intel's consumer line

* [Fixing Intel USB](https://usb-map.gitbook.io/project/)
* [Fixing CFG Lock](extras/msr-lock.md)


For sandy and Ivy Bridge:
* [Fixing Power Management](https://github.com/Piker-Alpha/ssdtPRGen.sh)

## Intel HEDT

Used for Intel's High End and Server line

* [Fixing Intel USB](https://usb-map.gitbook.io/project/)
* [Emulating NVRAM](/post-install/nvram.md)

For Sandy and Ivy Bridge E:
* [Fixing Power Management](https://github.com/Piker-Alpha/ssdtPRGen.sh)

## AMD

Used for AMD CPU based hardware

* [Fixing AMD USB](https://github.com/khronokernel/Opencore-Vanilla-Desktop-Guide/blob/master/AMD/AMD-USB-map.md)
* [Fixing AMD Temperature readings](https://github.com/trulyspinach/SMCAMDProcessor)
