# Lab 2: Windows 11 Pro Installation & Offline Setup

Welcome to **Lab 2**. This lab walks through the full, end-to-end Windows 11 Pro installation experience on physical hardware, bridging the gap between firmware configuration and the final operating system setup. 

You can interact with the live simulation here:
👉 [Windows 11 Pro Offline Setup Simulation](https://tibinjohn193-blip.github.io/windows-11/lab%202%20win11-pro-offline-setup-simulation%281%29.html)

---

## 🎯 Lab Objectives

1. **Pre-Installation & BIOS Navigation:** Master physical hardware handoff by configuring boot order via the motherboard BIOS/UEFI boot menu.
2. **USB Boot Media Handling:** Properly identify and boot from a physical USB installation medium (Kingston DataTraveler 3.0).
3. **Disk Partition Management:** Navigate disk selection, partition formatting, deletion, and creating new allocations.
4. **OOBE & Local Account Configuration:** Bypass forced Microsoft account requirements using the offline ("I don't have internet") workaround in Windows 11 Pro.

---

## 🔌 Phase 1: Boot Menu Selection & USB Connection (New in Lab 2)

Before Windows Setup launches, technicians must handle physical hardware handoff. This lab simulates that exact pre-installation sequence:

1. **Connect USB Drive:** Plug the bootable USB (e.g., *Kingston DataTraveler 3.0, 32GB*) into the target PC. The system confirms detection of a valid Windows 11 boot image.
2. **Restart & POST:** Trigger a system reboot into the motherboard manufacturer's POST (Power-On Self-Test) screen.
3. **Access Boot Menu:** Press the manufacturer-specific hotkey (`F12`, `F11`, `Esc`, or `Del`) during the memory test prompt to open the **BIOS Boot Menu**.
4. **Select Boot Device:** Choose `UEFI: Kingston DataTraveler 3.0 PMAP` from the blue-screen device list. Selecting incorrect items (like local Windows Boot Manager or network boot) correctly simulates hardware rejection.
5. **USB Hand-off:** Observe the `Booting from UEFI...` status message transitioning directly into the Windows Setup installer.

---

## 🖥️ Phase 2: Windows Setup & Partition Management

Once booted into the installer:
* **Language & Region:** Select your preferred language, time/currency format, and keyboard layout.
* **Setup Activation:** Click **Install Now** and input your product key (or select "I don't have a product key" for evaluation/later activation).
* **Edition Selection:** Choose **Windows 11 Pro**.
* **Disk Partitioning:**
  * View existing partitions on the target drive.
  * Practice **Delete**, **Format**, and **New** partition allocations.
  * Select the unallocated space or primary partition to begin file copying.
* **Installation Progress:** Watch the automated progress screen handle *Copying Windows files*, *Getting files ready for installation*, *Installing features*, *Installing updates*, and *Finishing up*.

---

## 👤 Phase 3: Out-of-Box Experience (OOBE) & Local Account Setup

Following the post-installation reboot, you enter the Windows 11 OOBE phase:
* Select your region, keyboard layout, and PC name.
* When prompted to connect to a network for Microsoft account sign-in, use the **Offline Workaround**:
  * Select **"I don't have internet"**.
  * Choose **"Continue with limited setup"**.
* Create a secure **Local User Account** (Username and Password) instead of being forced to link a cloud Microsoft account.
* Configure privacy settings (telemetry, location, diagnostics) to complete the setup and drop into the Windows 11 Pro desktop.

---

## 🛠️ Requirements & Troubleshooting

* **Media:** USB flash drive (minimum 8GB, formatted with Rufus or official Media Creation Tool).
* **Firmware:** UEFI mode enabled with Secure Boot compatible hardware profile.
* **Common Pitfall:** If the PC boots directly into the existing OS instead of the USB, verify your motherboard's boot menu key (`F12` is common on Dell/Intel, `F11` on MSI/ASRock, `F8` on ASUS).
