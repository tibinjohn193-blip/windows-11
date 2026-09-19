
# Lab 14: Windows 11 Advanced Firewall Management

This interactive lab demonstrates how to manage Windows Defender Firewall settings using both the basic Control Panel interface (`firewall.cpl`) and the Advanced Security interface (`wf.msc`). You will learn how to turn off the firewall for specific network profiles and how to create an Inbound Rule to block an incoming protocol on a specific port.

## 🛡️ Overview

Windows provides a two-tiered approach to managing network security:
1. **Control Panel (`firewall.cpl`):** Used for basic tasks like turning the firewall completely on/off for Private, Public, or Domain networks, and allowing basic apps through the firewall.
2. **Advanced Security (`wf.msc`):** Used by System Administrators to create highly granular rules (Inbound/Outbound) based on programs, ports, protocols (TCP/UDP), and IP addresses. 

In this lab, you will act as a System Administrator who needs to disable the basic firewall but block a specific developer port (TCP 8080) from incoming network traffic.

## 🎯 Lab Objectives

* Launch firewall tools directly using Windows Run commands.
* Turn off Windows Defender Firewall for both Private and Public network profiles.
* Navigate the Windows Defender Firewall with Advanced Security MMC snap-in.
* Create a custom **Inbound Rule** to block incoming connections.
* Filter traffic specifically for the **TCP protocol** on **Port 8080**.

## 📋 Step-by-Step Lab Instructions

Follow these steps within the interactive simulator to complete the lab:

### Part 1: Turn Off Basic Firewall (`firewall.cpl`)
1. Click the **Start Menu (🪟)**, search for `run`, and open the **Run** application.
2. Type `firewall.cpl` and click **OK** to open the Control Panel Firewall settings.
3. On the left pane, click **Turn Windows Defender Firewall on or off**.
4. Select **Turn off Windows Defender Firewall** under both the **Private** and **Public** network settings.
5. Click **OK**. Notice the firewall status changes to red (❌).

### Part 2: Block a Specific Port using Advanced Security
1. From the left menu in the Control Panel, click **Advanced settings** to open the Advanced Security console (`wf.msc`).
2. In the left pane, click on **📥 Inbound Rules**.
3. In the Actions pane on the far right, click **New Rule...** to open the Rule Wizard.
4. **Rule Type:** Select **Port** (to control connections for a TCP/UDP port) and click **Next**.
5. **Protocol and Ports:** Select **TCP**, choose **Specific local ports**, type `8080`, and click **Next**.
6. **Action:** Select **Block the connection** and click **Next**.
7. **Profile:** Ensure all profiles (Domain, Private, Public) are checked and click **Next**.
8. **Name:** Type `Block Port 8080` in the Name field and click **Finish**.
9. Verify that the new blocking rule (🚫) appears at the top of the Inbound Rules list.

---

## 💻 Interactive Lab

Test out your skills and run through the exact configuration steps in the interactive simulation below:

[**Click Here to Access Lab 14**](https://tibinjohn193-blip.github.io/windows-11/lab14.html)
