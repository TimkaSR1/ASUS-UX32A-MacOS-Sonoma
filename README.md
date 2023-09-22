# ASUS UX32A MacOS Sonoma

This EFI contains all the needed ACPI patches and kexts to make the ASUS UX32A run MacOS Sonoma/14.0

What works:
- Graphic acceleration (After applying OCLP patch)
- Wi-Fi
- Audio + Microphone
- Touchpad and keyboard
- Built-in display
- Battery indicator
- iCloud services (iMessage, Mail, Photos, etc)
- Sleep
- USB (Partially)

Installation guide:
Get MacOS Sonoma (Beta 7) image from [Olarila](https://www.olarila.com/files/?dir=Torrents)
Flash the image to a USB flash drive (16GB at least) or a external hard drive using [BalenaEtcher](https://etcher.balena.io)
Create a partition on your hard drive for MacOS (50GB at least and format the partitoin as NTFS so the installer can detect it)
Download this EFI and generate an SMBIOS (I used the MacBookAir8,2 SMBIOS but any supported SMBIOS will work)
Boot into MacOS
Go to disk utility and format the partition you created earlier as APFS
Go through the installation process
After installing the OS download [OCLP](https://nightly.link/dortania/OpenCore-Legacy-Patcher/workflows/build-app-wxpython/sonoma-development/OpenCore-Patcher.app%20%28GUI%29.zip) and apply the root patch
After this you should be done

Happy hackintoshing :3
