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

# Installation
Copy the CLOVER folder to your EFI

# Credits
I did very little work, mostly updating kexts and tinkering with configs for trackpad and sound
Credits go to @tylernguyen (Github), @rushstrike (tonymacx86), and @cabriolet (tonymacx86)
