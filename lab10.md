# Lab 10: Windows 11 Network Folder Sharing & Permissions (GUI)

This interactive lab demonstrates how to share a local folder over a network in Windows 11 using the Graphical User Interface (GUI). You will learn how to configure both Network Sharing permissions and NTFS Security permissions to ensure remote users can successfully access and modify the shared data.

## 📖 Overview

In a Windows network environment, simply clicking "Share" is often not enough. System administrators must configure **Advanced Sharing** to expose the folder to the network, and then configure **Security Permissions (NTFS)** to define exactly who can read, write, or execute files within that folder. This lab walks you through this exact two-step process.

## 🖥️ Lab Scenario & Topology

In this simulation, you will manage two Windows 11 machines on the same local network:

*   **PC1 (The Host):** 
    *   IP Address: `192.168.1.1`
    *   Credentials: `PC1` / `123`
*   **PC2 (The Client):** 
    *   IP Address: `192.168.1.2`

**Goal:** Create a folder named `SharedData` on PC1, share it with full permissions for everyone, and access it remotely from PC2 using its UNC path.

---

## 📋 Step-by-Step Lab Instructions

Follow these steps within the simulator to complete the lab:

### Part 1: Verify Connectivity & Create Folder (On PC1)
1. Open **Command Prompt** from the Start menu and type `ping 192.168.1.2` to ensure PC1 can communicate with PC2.
2. Open **File Explorer** and navigate to **Local Disk (C:)**.
3. Right-click the empty space, select **New > Folder**, and rename it exactly to `SharedData`.

### Part 2: Configure Advanced Sharing (On PC1)
1. Right-click the `SharedData` folder and select **Properties**.
2. Go to the **Sharing** tab and click **Advanced Sharing...**.
3. Check **Share this folder** and click **Permissions**.
4. Check the **Full Control** box under Allow. 
5. Click **Apply**, then **OK**, and click **OK** again to close the Advanced Sharing dialog.

### Part 3: Configure NTFS Security Permissions (On PC1)
1. In the folder Properties window, switch to the **Security** tab and click **Edit...**.
2. Click **Add...**, type `Everyone` in the object names box, and click **OK**.
3. Select **Everyone** from the list, and check **Full control** under Allow.
4. Click **Apply**, then **OK**, and finally **OK** on the main Properties window.

### Part 4: Access the Shared Folder (From PC2)
1. Use the top toggle button to switch to **View PC2**.
2. Click **Start**, search for the **Run** app, and open it.
3. Type the UNC path of the host machine: `\\192.168.1.1` and click **OK**.
4. When prompted by Windows Security, enter PC1's network credentials (Username: `PC1`, Password: `123`).
5. **Success!** File Explorer will open displaying the shared `SharedData` folder over the network.

---

## 💻 Interactive Lab

Test out your skills and run through the exact configuration steps in the interactive simulation below:

[**Click Here to Access Lab 10**](https://tibinjohn193-blip.github.io/windows-11/lab10.html)
