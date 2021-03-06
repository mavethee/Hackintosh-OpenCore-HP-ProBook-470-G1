<img src="https://github.com/acidanthera/OpenCorePkg/blob/master/Docs/Logos/OpenCore_with_text_Small.png" width="200" height="48"/>

## Hackintosh-OpenCore-HP-ProBook-470-G1
EFI premade of OpenCore bootloader for HP ProBook 470 G1 is here!

## Current version - OpenCore 0.6.5 (4th January)
Repository contains full ,,Plug-and-Play" EFI of OpenCore bootloader and
all needed files to install and run macOS on HP ProBook 470 G1!

https://github.com/acidanthera/OpenCorePkg/releases/tag/0.6.5

## Important note:
EFI premade is done for people with Intel and Broadcom WiFi Bluetooth cards!
Since OC 0.6.5, I decided to switch to RELEASE version, if you expierience any issues, switch to debug using Dortania's Guide:

https://dortania.github.io/OpenCore-Install-Guide/troubleshooting/debug.html

My main DELL-7567 fried so won't be able keep up to date this repo anymore,
planning to get ThinkPad x240 and continue Hackintosh repos soon.

### SMBIOS:
Present in repo SMBIOS is not purchased Apple's device but for own sake, I don't advice you to use it.
...for own sake ;)

To generate SMBIOS you can use:
* OpenCore Configurator: 
https://mackie100projects.altervista.org/download-opencore-configurator/
* Clover Configurator:
https://mackie100projects.altervista.org/download-clover-configurator/

Tool doesn't matter really, you just need not valid or unused SMBIOS to copy-paste needed info.
...if you wish to use iServices of course :)

### If you use Intel:
Delete all Brcm kexts from EFI/OC/Kexts, 
Depending on macOS version, you're planning to use:
* Airportitlwm_Big_Sur for macOS 11 Big Sur,
* Airportitlwm_Catalina for macOS 10.15 Catalina,
* Airportitlwm_Mojave for macOS 10.14 Mojave,
* Airportitlwm_High_Sierra for macOS 10.13 High Sierra.
After that rename chosen Airportitlwm kext to Airportitlwm.kext

And then make a snapshot of config.plist in ProperTree!

### If you use Broadcom: 
Delete all Intel kexts from EFI/OC/Kexts

Depending on macOS version, you're planning to use:
* BrcmPatchRAM3 for 10.14+ (must be paired with BrcmBluetoothInjector)
* BrcmPatchRAM2 for 10.11-10.14
* BrcmPatchRAM for 10.8-10.10

And then, make a snapshot of config.plist in ProperTree!


## Credits:

### Airportitlwm (1.1.0):
https://github.com/OpenIntelWireless/itlwm
### AppleALC (1.5.6):
https://github.com/acidanthera/AppleALC
### Broadcom (Optional, for people who replaced Intel with it):
https://github.com/acidanthera/BrcmPatchRAM/

https://github.com/acidanthera/AirportBrcmFixup/
### CPU Friend (1.2.3):
https://github.com/acidanthera/CPUFriend/
### HibernationFixup (1.3.9):
https://github.com/acidanthera/HibernationFixup/
### IntelBluetoothFirmware (1.1.2):
https://github.com/OpenIntelWireless/IntelBluetoothFirmware
### Lilu (1.5.0):
https://github.com/acidanthera/Lilu/
### NVMeFix (1.0.5):
https://github.com/acidanthera/NVMeFix
### RealtekRTL8111 (2.3.0):
https://github.com/Mieze/RTL8111_driver_for_OS_X
### USBInjectAll (0.7.1):
https://bitbucket.org/RehabMan/os-x-usb-inject-all/downloads
### VirtualSMC (1.1.9):
https://github.com/acidanthera/VirtualSMC
### VoodooInput (1.0.9):
https://github.com/acidanthera/VoodooInput
### VoodooPS2 (2.2.0):
https://github.com/acidanthera/VoodooPS2
### WhateverGreen (1.4.6):
https://github.com/acidanthera/WhateverGreen
### OpenCanopy's resources:
https://github.com/acidanthera/OcBinaryData

## Thanks for using my EFI premade, I would be glad for some feedback! :)
