# x1c6-macOS
macOS Catalina (10.15) for the ThinkPad X1 Carbon 6th Gen

Big thanks to @tylernguyen

# Specs
|    CPU   |   GPU   |  RAM  | STORAGE |    DISPLAY    |
|:--------:|:-------:|:-----:|:-------:|:-------------:|
| i7-8550u | UHD 620 | 16 GB |  512 GB | 2560x1440 HDR |

# Summary
| Working                          | Not Working                   | Not Sure                    |
|----------------------------------|-------------------------------|-----------------------------|
| USB A, C Audio, Sleep*, Graphics | Fingerprint (Disable in BIOS) | Thunderbolt 3 Functionality |
| Trackpoint                       | WWAN (Disable in BIOS)        |                             |
| Mostly Stable OS                 | SD Reader (Disable in BIOS)   |                             |
| USB-C to Displayport             |                               |                             |

* Sleep itself is working very well, but the power button and Thinkpad LED still blink, even if awake

The provided wifi card is not compatible with macOS, so I would recommend the DW1560

# BIOS Configuration
Enable thunderbolt assist in BIOS for better power management, and maybe disable VT-D. Disable the devices above, 

# Installation
Copy the folders to your EFI, and things should work for the most part.

# Troubleshooting
Some issues may occur due to hardware differences

## Audio
If your audio is not working, switch layout-id in ``config.plist`` to ``0B000000`` or ``1F000000``

## Power Management
Even though you may or may not have the same CPU, their configuration/profiles may be different, so generate new CPUFriend kexts for better PM.

# Credits
I did very little work, mostly updating kexts and tinkering with configs for trackpad and sound
Credits go to @tylernguyen (Github), @rushstrike (tonymacx86), and @cabriolet (tonymacx86)
