
# Windows 11 Disk Management 
---

## 📚 Core Concepts: Partition Styles & File Systems

When managing disks in Windows, understanding how the drive is initialized (Partition Style) and formatted (File System) is crucial. This simulation helps visualize the actions that take place on top of these foundational concepts.

### 1. Partition Styles: MBR vs. GPT
Before a disk can be formatted, it must be initialized with a partition style that tells Windows how data is organized on the drive.

* **MBR (Master Boot Record):**
  * The older, legacy standard.
  * **Limitations:** Only supports disk sizes up to **2 TB**.
  * **Partitions:** Supports a maximum of only **4 Primary Partitions**. If more are needed, one must be converted into an "Extended Partition" to hold "Logical Drives."
* **GPT (GUID Partition Table):**
  * The modern standard (Required for Windows 11 and modern UEFI systems).
  * **Advantages:** Supports massive disk sizes (up to 18 Exabytes).
  * **Partitions:** Supports up to **128 Primary Partitions** natively in Windows.
  * More resilient to data corruption as it stores multiple copies of the partition data across the disk.

### 2. Windows File Systems: NTFS, FAT32 & exFAT
Once a partition is created (as seen in the "New Simple Volume" step of the simulation), it must be formatted with a File System.

* **NTFS (New Technology File System):**
  * The default and preferred file system for modern Windows internal drives (used in this simulation to format the new E: drive).
  * **Features:** Supports huge file sizes and partition sizes. Includes advanced security features like file/folder-level permissions, encryption (EFS), compression, and journaling (which helps recover data if the system crashes).
* **FAT32 (File Allocation Table 32):**
  * A legacy file system still heavily used for USB flash drives and SD cards due to its universal compatibility across Windows, macOS, Linux, and gaming consoles.
  * **Limitations:** The maximum file size you can store is **4 GB** (a single file cannot exceed this). Windows limits formatting FAT32 partitions to a maximum of 32 GB.
* **exFAT (Extended FAT):**
  * Created by Microsoft specifically for flash drives to bridge the gap between FAT32 and NTFS.
  * **Features:** Removes the 4 GB file size limit of FAT32 while maintaining excellent cross-platform compatibility (works natively on modern macOS and Windows) without the heavy overhead of NTFS.

---


# Windows 11 Disk Management Simulation 💽

An interactive, browser-based simulation of the Windows 11 Disk Management utility (`diskmgmt.msc`). This project is designed for educational purposes and lab environments, allowing users to safely practice disk provisioning, partitioning, and volume management without making any changes to physical hardware.

## 🚀 Features Demonstrated in this Simulation
* **Shrink Volume:** Safely reduce the size of a primary partition (C:) to create Unallocated space.
* **New Simple Volume Wizard:** Step-by-step creation of a new partition (E:) including assigning drive letters and formatting.
* **Delete Volume:** Simulating the removal of a partition to free up space.
* **Extend Volume:** Adding unallocated space back to an existing primary partition.
* **File Explorer Integration:** Verifying partition creation dynamically in a simulated "This PC" environment.

  
## 🛠️ How to Use the Simulation

1. Clik the Acess Lab Button in Below
2. Follow the on-screen instructions in the blue panel at the top.
3. Interact with the Windows 11 UI, use the 'Run' dialog, and right-click on the disk blocks to perform actions.

[ACESS LAB]()
