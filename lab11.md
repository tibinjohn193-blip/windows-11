# Lab 11: Windows 11 Malicious Software Removal Tool (MRT) Scan

This interactive lab demonstrates how to manually launch and run the Microsoft Malicious Software Removal Tool (MSRT) using the Windows 11 Run dialog. You will learn how to navigate User Account Control (UAC) prompts and execute a system scan to check for prevalent malware.

## 🛡️ What is the Malicious Software Removal Tool (MRT)?

The **Microsoft Malicious Software Removal Tool (MSRT)** is a built-in, free utility provided by Microsoft that scans computers running Windows for specific, prevalent malicious software (such as Blaster, Sasser, and Mydoom) and helps remove the infection if found. 

### 📌 Key Features
* **Built-in Utility:** Pre-installed on Windows systems; no separate download or installation is required to run it manually.
* **Regular Updates:** Microsoft releases an updated version of this tool on the second Tuesday of every month (Patch Tuesday) via Windows Update.
* **Targeted Detection:** It specifically targets known, high-risk malware families rather than acting as a general-purpose scanner.
* **Multiple Scan Modes:** Offers Quick Scan (critical system areas), Full Scan (entire system), and Customized Scan (specific folders).
* **Silent Execution:** Usually runs quietly in the background after a Windows Update, but can be triggered manually via the `mrt` command.

### ⚠️ Important Note on Uses
**MRT is NOT a replacement for a full antivirus program** (like Windows Defender or third-party AVs). 
* It **does not** provide real-time protection.
* It **does not** prevent malware from entering the system.
* It is exclusively used for **post-infection cleanup** of specific, widespread threats.

---

## 🎯 Lab Objectives

1. Launch the Windows **Run** application via the Start Menu Search.
2. Execute the `mrt` command to open the tool.
3. Handle Windows **User Account Control (UAC)** elevation prompts.
4. Navigate the MRT Wizard and initiate a **Quick Scan**.
5. Analyze the scan process and review the final malware detection results.

---

## 📋 Step-by-Step Lab Instructions

Follow these steps within the interactive simulator to complete the lab:

### Part 1: Launch the Tool
1. Click the **Start Menu (🪟)**.
2. Type `run` in the search box and click the **Run** app from the results.
3. In the Run dialog box, type `mrt` and click **OK**.
4. A **User Account Control (UAC)** prompt will appear asking for administrator privileges. Click **Yes** to allow the tool to make changes to your device.

### Part 2: Execute the Scan
1. The **MRT Wizard** will open. Read the Welcome screen and click **Next**.
2. You will be prompted to choose a scan type. Select **Quick scan** (which checks the areas of the system most likely to contain malicious software) and click **Next**.
3. The tool will begin scanning your computer. You can observe the progress bar, files scanned, and the current file path being checked (e.g., `C:\Windows\System32\hal.dll`).
4. Wait a few moments for the scan simulation to complete.

### Part 3: Review Results
1. Once the scan finishes, the results screen will appear.
2. Verify the message: **"No malicious software was detected."**
3. Click **Finish** to close the tool and complete the lab.

---

## 💻 Interactive Lab

Test out your skills and run through the exact configuration steps in the interactive simulation below:

[**Click Here to Access Lab 11**](https://tibinjohn193-blip.github.io/windows-11/lab11.html)
