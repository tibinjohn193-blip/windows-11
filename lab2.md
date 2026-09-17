#  lab 2 win11-pro-offline-setup-simulation(1).html

Walks through the full installer experience end to end: language/keyboard/license screens, disk partition selection (Format, Delete, New), the "Installing Windows" progress screen, and the complete first-boot (OOBE) flow — including the Wi-Fi screen's "I don't have internet" path that lets Windows 11 Pro set up a local account instead of requiring a Microsoft account.


## 🔌 Boot Menu Selection & USB Connection (new in Lab 2)

Before the Windows Setup screens even appear, the lab now walks through the real pre-installation sequence a technician goes through on physical hardware:

Connect the USB drive — click to plug the bootable USB (a Kingston DataTraveler 3.0, 32GB) into the PC. The simulation confirms detection and shows that it contains a bootable Windows 11 image.
Restart the PC — triggers a short "Restarting…" spinner, mimicking the reboot needed to get into firmware.
BIOS/UEFI splash screen — a classic black POST screen showing the motherboard manufacturer, BIOS version, CPU, and memory test, with a blinking prompt: "Press [F12] for Boot Menu." Clicking it simulates hitting the boot menu hotkey during POST (the exact key varies by manufacturer — F12, F11, Esc, or Del are common).
BIOS Boot Menu — a proper blue-screen BIOS boot device list, letting you select between the local disk's Windows Boot Manager, the USB drive (shown exactly as firmware reports it: UEFI: Kingston DataTraveler 3.0 PMAP), onboard network boot (IPv4/IPv6), or entering BIOS Setup. Selecting anything other than the USB and pressing Enter does nothing (just like a real BIOS would ignore an incompatible choice for this scenario) — only selecting the USB drive and confirming boots into the installer.
Booting from USB — a brief "Booting from UEFI: Kingston DataTraveler 3.0 PMAP..." message before handing off into the familiar Windows Setup language screen.

This section exists because in the real world, getting a PC to boot from USB is often the part people get stuck on — not because Windows Setup is hard, but because finding the right boot-menu key and correctly identifying the USB drive among BIOS entries trips people up. The lab lets you practice that exact decision point risk-free.

[installing win 11 pro](https://tibinjohn193-blip.github.io/windows-11/lab%202%20win11-pro-offline-setup-simulation%281%29.html)
