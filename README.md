# ASUS UX32A MacOS Sonoma

This EFI contains all the needed ACPI patches and kexts to make the ASUS UX32A run MacOS Sonoma/14.0

ASUS UX32A Specs:
- CPU: Intel Core i5-3317U
- GPU: Intel HD 4000 Graphics (Ivy Bridge)
- Speakers: Realtek ALC269VB
- Display: 1366x768

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
- Get MacOS Sonoma (Beta 7) image from [Olarila](https://www.olarila.com/files/?dir=Torrents)
- Flash the image to a USB flash drive (16GB at least) or a external hard drive using [BalenaEtcher](https://etcher.balena.io)
- Create a partition on your hard drive for MacOS (50GB at least and format the partitoin as NTFS so the installer can detect it)
- Download this EFI and generate an SMBIOS (I used the MacBookAir8,2 SMBIOS but any supported SMBIOS will work)
- Boot into MacOS
- Go to disk utility and format the partition you created earlier as APFS
- Go through the installation process
- After installing the OS download [OCLP](https://nightly.link/dortania/OpenCore-Legacy-Patcher/workflows/build-app-wxpython/sonoma-development/OpenCore-Patcher.app%20%28GUI%29.zip) and apply the root patch
After this you should be done

Credits:
- [Apple](apple.com) for MacOS
- [Olarila](olarila.com) for the MacOS images and original EFI folder
- [ASUS UX32VD Hackintosh](https://github.com/rafaelmaeuer/Asus-UX32VD-Hackintosh) for the ACPI patches
- [OpenIntelWireless](https://github.com/OpenIntelWireless) for [Itlwm](https://github.com/OpenIntelWireless/itlwm)
- [Acidanthera](https://github.com/acidanthera) for [OpenCore](https://github.com/acidanthera/OpenCorePkg), [Lilu](https://github.com/acidanthera/Lilu), [WhateverGreen](https://github.com/acidanthera/WhateverGreen), [VirtualSMC](https://github.com/acidanthera/VirtualSMC), [VoodooPS2](https://github.com/acidanthera/VoodooPS2), [AppleALC](https://github.com/acidanthera/AppleALC), [CryptexFixup](https://github.com/acidanthera/CryptexFixup)
- [dortania](https://github.com/dortania) for [OpenCore Legacy Patcher](https://github.com/dortania/OpenCore-Legacy-Patcher) and the [OpenCore Install Guide](https://dortania.github.io/OpenCore-Install-Guide)
- [5T33Z0](https://github.com/5T33Z0) for the [MacOS Ventura and higher install guide](https://github.com/5T33Z0/OC-Little-Translated/blob/main/14_OCLP_Wintel/Ivy_Bridge-Ventura.md)

Happy hackintoshing :3

![Screenshot 2023-09-22 at 8 36 28 PM](https://github.com/TimkaSR1/ASUS-UX32A-MacOS-Sonoma/assets/143961127/fa2cf6eb-d772-41ce-b3b4-abcce98ab97f)

