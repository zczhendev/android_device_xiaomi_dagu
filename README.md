# android_device_xiaomi_dagu

Xiaomi Pad 5 Pro 12.4 (dagu) Device Tree for LineageOS 23.2

## How to flash

You will lose all user data after flashing LineageOS. Remember to back it up in a safe place. I warned you.

1. Unlock your bootloader & Flash HyperOS first (matching the firmware base used for vendor blobs)
2. Download `boot.img`, `vendor_boot.img` and `lineage-<version>-UNOFFICIAL-dagu.zip` from GitHub release
3. Reboot to bootloader mode, flash boot and vendor_boot by `fastboot flash boot boot.img && fastboot flash vendor_boot vendor_boot.img`
4. Reboot to recovery mode, do Factory reset, click "Apply update -> Apply from ADB" and `adb sideload lineage-<version>-UNOFFICIAL-dagu.zip`
5. Reboot
