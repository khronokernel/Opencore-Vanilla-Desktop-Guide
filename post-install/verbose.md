# Fixing Resolution and Verbose

* Supported version: 0.5.7

**Attention to all users, please note this guide and other khronokernel sites will be shutting down on April 16th, 2020. Reason for this is we've decided to move the guides to a dedicated organization to help simplify the hackintosh process and provide a single, trusted source for hackintosh information. This new organization will be known as [Dortania](https://github.com/dortania).**

Links to the new sites:

* [OpenCore Desktop Guide](https://dortania.github.io/OpenCore-Desktop-Guide/)
* [Getting Started with ACPI](https://dortania.github.io/Getting-Started-With-ACPI/)
* [GPU Buyers Guide](https://dortania.github.io/GPU-Buyers-Guide/)
* [Wireless Buyers Guide](https://dortania.github.io/Wireless-Buyers-Guide/)
* [Anti-Hackintosh Buyers Guide](https://dortania.github.io/Anti-Hackintosh-Buyers-Guide/)

Wanting a more clean booting experience with macOS without all that verbose text while booting? Well you need a couple things:

## Recommended Configuration:

**`NVRAM -> 7C436110-AB2A-4BBB-A880-FE41995C9F82 -> boot-args`**:

* Remove `-v` from your config.plist

**`NVRAM -> 4D1EDE05-38C7-4A6A-9CC6-4BCCA8B38C14 -> UIScale`**:

* `01`: Standard resolution
* `02`: HiDPI (generally required for FileVault to function correctly on smaller displays)


**`UEFI -> Output`**:

* `TextRenderer` set to`BuiltinGraphics`
* `Resolution`: set to `Max` for best results
   * Optionally can specify resolution: `WxH@Bpp (e.g. 1920x1080@32) or WxH (e.g. 1920x1080)`
* `ProvideConsoleGop` set to True


If still having issues, see [Configuration.pdf](https://github.com/acidanthera/OpenCorePkg/blob/master/Docs/Configuration.pdf) for all possible options.
