# Moving OpenCore from USB to macOS Drive

* Supported version: 0.5.7

**Attention to all users, please note this guide and other khronokernel sites will be shutting down on April 16th, 2020. Reason for this is we've decided to move the guides to a dedicated organization to help simplify the hackintosh process and provide a single, trusted source for hackintosh information. This new organization will be known as [Dortania](https://github.com/dortania).**

Links to the new sites:

* [OpenCore Desktop Guide](https://desktop.dortania.ml/)
* [Getting Started with ACPI](https://acpi.dortania.ml/)
* [GPU Buyers Guide](https://gpu.dortania.ml/)
* [Wireless Buyers Guide](https://wifi.dortania.ml/)
* [Anti-Hackintosh Buyers Guide](https://hardware.dortania.ml/)

## Grabbing OpenCore off the USB

So to start, we'll first want to grab OpenCore off of our installer. To do this, we'll be using a neat tool from CorpNewt called [MountEFI](https://github.com/corpnewt/MountEFI)

For this example, we'll assume your USB is called `Install macOS Catalina`:

![](https://cdn.discordapp.com/attachments/683011276938543134/684629962539663390/Screen_Shot_2020-03-03_at_10.13.56_PM.png)

Once the EFI's mounted, we'll want to grab our EFI folder on there and keep in a safe place. We'll then want to **eject the USB drive's EFI** as having multiple EFIs mounted can confuse macOS sometimes, best practice is to keep only 1 EFI mounted at a time(you can eject just the EFI, the drive itself doesn't need to be removed)

![](https://cdn.discordapp.com/attachments/683011276938543134/684634974753652970/Screen_Shot_2020-03-03_at_10.34.15_PM.png)

Now with this done, lets mount our macOS drive. With macOS Catalina, macOS is actually partitioned into 2 volumes: System Partition and User Partition. This means that MountEFI may report multiple drives in it's picker but each partition will still share the same EFI(The UEFI spec only allows for 1 EFI per drive). You can tell if it's the same drive with disk**X**sY (Y is just to say what parition it is)

![](https://cdn.discordapp.com/attachments/683011276938543134/684635377297915932/Screen_Shot_2020-03-03_at_10.22.20_PM.png)

When you mount your main drive's EFI, you may be greeted with a folder called `APPLE`, this is used for updating the firmware on real Macs but has no effect on our hardware. You can wipe everything on the EFI partition and replace it with the one found on your USB


## Special notes for legacy users

When transfering over your EFI, there are still boot sectors that need to be written to so your non-UEFI BIOS would be able to find it So don't forget to rerun the [`BootInstall.command`](/extras/legacy.md) on your macOS drive


