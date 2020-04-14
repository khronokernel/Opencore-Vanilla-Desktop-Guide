# Making the installer with an Android Phone

* Supported version: 0.5.7

**Attention to all users, please note this guide and other khronokernel sites will be shutting down on April 16th, 2020. Reason for this is we've decided to move the guides to a dedicated organization to help simplify the hackintosh process and provide a single, trusted source for hackintosh information. This new organization will be known as [Dortania](https://github.com/dortania).**

Links to the new sites:

* [OpenCore Desktop Guide](https://dortania.github.io/OpenCore-Desktop-Guide/)
* [Getting Started with ACPI](https://dortania.github.io/Getting-Started-With-ACPI/)
* [GPU Buyers Guide](https://dortania.github.io/GPU-Buyers-Guide/)
* [Wireless Buyers Guide](https://dortania.github.io/Wireless-Buyers-Guide/)
* [Anti-Hackintosh Buyers Guide](https://dortania.github.io/Anti-Hackintosh-Buyers-Guide/)

(This is a joke, you can follow this but you really should just buy a $3 USB)


**Requirements:**

* Rooted Android phone with [DriveDroid](https://softwarebakery.com/projects/drivedroid)
* macOS Recovery files

1. Partition your Drive into 2 parts:
* 200MB partition named EFI
* 4GB partition for macOS install

2. Create a folder on the 4GB partition called `com.apple.recovery.boot` and add the following inside it:
* recovery file(.dmg)
* chunklist file(.chunklist)

3. [Create your OpenCore EFI](/installer-guide/opencore-efi.md)

4. Boot

