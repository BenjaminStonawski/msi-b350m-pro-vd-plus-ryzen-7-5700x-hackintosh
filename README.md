# OpenCore 1.0.4
## Specs
| **Component**    | **Model**                         |
| ---------------- | --------------------------------- |
| CPU              | AMD Ryzen 7 5700X @ 3.4GHz        |
| Motherboard      | MSI B350M PRO-VD PLUS             |
| RAM              | 16GB (2 x 8GB) G.Skill @ 2133MHz  |
| GPU              | GIGABYTE RX 5700 XT GAMING OC 8G  |
| Audio Chipset    | Realtek® ALC887 Codec             |
| Ethernet (LAN)   | Realtek® 8111H Gigabit LAN        |
| WiFi & Bluetooth | Fenvi T919 (BCM94360CD)           |
| OS Disk          | KINGSTON SA400S37480G (SATA)      |
| Current OS       | macOS Sequoia 15.4.1 (24E263)     |

## Things to know
<b>To get Fenvi T919 working, you'll need to do some trickery as Apple dropped support for Broadcom cards since Sonoma. There are multiple guides online, I found [this one](https://github.com/perez987/Fenvi-T919-wifi-back-on-macOS-Sonoma-with-OCLP) the most useful</b><br><br>
<b>Use [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS) to generate a serial number and a MLB (motherboard serial number) for MacPro7,1. In the config.plist the entries of the serial number and MLB are empty! You'll also need to generate the System-UUID and the ROM in SMBIOS, I recommend generating it with [OCAT](https://github.com/ic005k/OCAuxiliaryTools)</b><br><br>
<b>With AMD CPUs, a lot of applications will crash or won't function properly, that's due to MKL, to fix this, I highly recommend [amdfriend](https://github.com/NyaomiDEV/AMDFriend) to fix these issues!</b><br><br>
If Handoff or Universal Clipboard don't work, check out my guide in the 'handoff-fix' folder!

## What works
✅ Ethernet + WiFi + Bluetooth => AirDrop, Handoff, iMessage/FaceTime <br>
✅ Graphics Acceleration (RX 5700 XT is natively supported)<br>
✅ AMD Power Management<br>
✅ Sleep mode<br>
✅ All audio ports (front and rear speaker/mic ports, HDMI/DP audio) => Boot Chime<br>
✅ USB ports<br>

## Doesn't work
🫢 Well, everything works!
