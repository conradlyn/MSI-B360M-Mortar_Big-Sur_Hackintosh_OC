# MSI B360M Mortar with Big Sur
Fully functioning OpenCore EFI for MSI B360M Mortar at **macOS Big Sur**

### OpenCore: 0.6.0
### macOS Big Sur (Public Beta 1)

## Hardware
- **CPU:** Intel i5 9400
- **MB:** MSI B360M Mortar
- **GPU:** Sapphire RX 5500 XT 8GB
- **Display:** AOC U2790 (27 inches, 3840x2160) via dp
- **RAM:** Kingston 16GB
- **SSD:** Intel NVME 256GB
- **Wifi + Bluetooth:** BCM943602CS

Another SSD (Samsung 860 Evo) is installed for Windows 10. OC set to boot macOS as default. I use function key F11 to boot Windows 10 from the Samsung SSD.
Windows 10 also can be booted directly from OC (tested).

## Caveat

- You need to fill in the **platforminfo** by yourself.
- You may want to generate your own **CPUFriendDataProvider.kext**. Alternatively, you can delete CPUFriend.kext and CPUFriendDataProvider.kext all together, and disable / delete the corresponding entries in config.plist.
- You may want to generate your own **USBPorts.kext** or use USBInjectAll.kext (mutually exclusive).
- You can also delete **IntelMausi.kext** if ethernet is not needed, and disable / delete the entry in config.plist.

(remember to rebuild cache if kexts are deleted)
