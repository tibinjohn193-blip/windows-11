# Lab: Configuring Static IPs & Network Connectivity

This lab guides you through the process of manually assigning a static IP address to your computer using the Windows Network Connections control panel (`ncpa.cpl`). After configuring the IP, you will test connectivity to a second PC on the network.

## 🖥️ Lab Topology

To ensure proper communication without IP conflicts, each device must have a unique address:
*   **PC1 (Your Machine):** IP Address `192.168.1.1`
*   **PC2 (Target Machine):** IP Address `192.168.1.2`
*   **Subnet Mask:** `255.255.255.0` 

## 🎯 Lab Objectives

*   Use the `ncpa.cpl` shortcut to quickly access Network Connections.
*   Configure a static IPv4 address and Subnet Mask via the Windows GUI.
*   Verify the new IP configuration using Command Prompt.
*   Use ICMP `ping` to verify communication with a second PC.

---

## 📋 Step-by-Step Instructions PC1

### Part 1: Assign a Static IP using `ncpa.cpl`
1. **Open Network Connections:** 
   * Press `Windows Key + R` on your keyboard to open the Run dialog box.
   * Type `ncpa.cpl` and press **Enter**.
2. **Access Adapter Properties:**
   * Right-click on your active network adapter (usually named **Ethernet** or **Wi-Fi**) and select **Properties**.
3. **Open IPv4 Settings:**
   * In the list of items, locate and click on **Internet Protocol Version 4 (TCP/IPv4)** to highlight it.
   * Click the **Properties** button below the list.
4. **Enter the IP Details:**
   * Select the radio button for **"Use the following IP address"**.
   * **IP address:** Enter `192.168.1.1`
   * **Subnet mask:** Enter `255.255.255.0` (this usually auto-fills when you click the box).
   * Leave the Default Gateway blank for this local-only lab.
5. **Save Changes:**
   * Click **OK** on the IPv4 properties window, then click **Close** on the Ethernet properties window to apply the settings.

## 📋 Step-by-Step Instructions PC2

### Part 1: Assign a Static IP using `ncpa.cpl`
1. **Open Network Connections:** 
   * Press `Windows Key + R` on your keyboard to open the Run dialog box.
   * Type `ncpa.cpl` and press **Enter**.
2. **Access Adapter Properties:**
   * Right-click on your active network adapter (usually named **Ethernet** or **Wi-Fi**) and select **Properties**.
3. **Open IPv4 Settings:**
   * In the list of items, locate and click on **Internet Protocol Version 4 (TCP/IPv4)** to highlight it.
   * Click the **Properties** button below the list.
4. **Enter the IP Details:**
   * Select the radio button for **"Use the following IP address"**.
   * **IP address:** Enter `192.168.1.2`
   * **Subnet mask:** Enter `255.255.255.0` (this usually auto-fills when you click the box).
   * Leave the Default Gateway blank for this local-only lab.
5. **Save Changes:**
   * Click **OK** on the IPv4 properties window, then click **Close** on the Ethernet properties window to apply the settings.
  

### Part 2: Verify and Ping PC2
1. **Open Command Prompt:** 
   * Press `Windows Key + R`, type `cmd`, and press **Enter**.
2. **Ping the Second PC:** 
   * Type `ping 192.168.1.2` and press **Enter**.
3. **Analyze the Results:**
   * If the configuration is correct, you will see `Reply from 192.168.1.2` along with a `0% loss` statistic, indicating the two PCs are successfully talking to each other.

---

## 💻 Interactive Lab

Test out your skills and run through the exact configuration steps in the interactive simulation below:

[**Click Here to Access the Lab Simulation**](https://tibinjohn193-blip.github.io/windows-11/lab6.html)
