# Lab 7: Windows 11 Remote Desktop Connection (RDP)

This interactive lab demonstrates how to configure and use the Remote Desktop Connection feature in Windows 11. You will learn how to verify network connectivity, enable remote access in Windows Settings, and establish a remote session between two computers.

## 📖 What is Remote Desktop?

**Remote Desktop Protocol (RDP)** is a built-in Windows feature that allows you to connect to and control a PC from another device over a network or the internet. 

When you connect via RDP, you see the remote computer's screen on your local monitor and can use your own keyboard and mouse to control it, exactly as if you were sitting directly in front of it. It is widely used by IT administrators for remote troubleshooting and by users accessing their work computers from home.

## 🖥️ Lab Scenario & Topology

In this simulation, you will manage two Windows 11 machines on the same local network:

*   **PC1 (The Host / Target):** 
    *   IP Address: `192.168.1.1`
    *   Username: `PC1`
    *   Password: `1234`
*   **PC2 (The Client):** 
    *   IP Address: `192.168.1.2`

**Goal:** Successfully connect *from* PC2 *to* PC1 using Remote Desktop.

---

## 📋 Step-by-Step Lab Instructions

Follow these steps within the simulator to complete the lab:

### Part 1: Verify Connectivity (On PC1)
Before attempting a remote connection, you must ensure the two computers can talk to each other.
1. Make sure you are viewing **PC1**.
2. Click the **Start Menu (🪟)** and open **Command Prompt (⬛)**.
3. Type `ping 192.168.1.2` and press Enter to verify PC1 can reach PC2.
4. Close the Command Prompt.

### Part 2: Enable Remote Desktop (On PC1)
By default, Windows blocks incoming Remote Desktop connections for security reasons. You must enable it on the target machine.
1. Click the **Start Menu (🪟)** and open **Settings (⚙️)**.
2. In the Settings search bar, type `Remote` and select **Remote Desktop settings**.
3. Toggle the **Remote Desktop** switch to **On**. PC1 is now listening for incoming connections.

### Part 3: Enable Remote Desktop (On PC2)
1. Use the toggle button at the top of the screen to switch to **View PC2 (192.168.1.2)**.
2. Open **Settings (⚙️)** from the Start Menu.
3. Search for Remote Desktop and toggle it **On** for PC2 as well.

### Part 4: Initiate the Connection (From PC2 to PC1)
Now that both machines are configured, you will launch the RDP client on PC2.
1. Click the **Start Menu (🪟)** and click the **Run (🏃)** app (This simulates pressing `Win + R`).
2. In the Run dialog box, type `mstsc` (the executable name for Microsoft Terminal Services Client) and click **OK**.
3. The Remote Desktop Connection window will open. Enter PC1's IP address: `192.168.1.1` and click **Connect**.

### Part 5: Authentication & Security
1. A Windows Security prompt will appear asking for credentials.
2. Enter the target PC's credentials:
   *   **Username:** `PC1`
   *   **Password:** `1234`
3. Click **OK**.
4. You will see a security warning stating that the identity of the remote computer cannot be verified. Click **Yes** to accept the certificate and connect.
5. **Success!** You will now see PC1's screen operating inside a window on PC2.

---

## 💻 Interactive Lab

Test out your skills and run through the exact configuration steps in the interactive simulation below:

[**Click Here to Access Lab 7**](https://tibinjohn193-blip.github.io/windows-11/lab7.html)
