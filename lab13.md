
# Lab 13: Windows 11 BitLocker Recovery Key Unlock

This interactive scenario-based lab demonstrates how to regain access to a BitLocker-encrypted drive when the unlock password is forgotten. You will learn how to locate a saved recovery key, use the 48-digit key to bypass the password prompt, and access the full BitLocker management settings to disable encryption.

## 🔑 What is a BitLocker Recovery Key?

A BitLocker recovery key is a unique 48-digit numerical password that can be used to unlock your system if BitLocker is unable to confirm for certain that the attempt to access the system drive is authorized, or if the user forgets their standard password. 

### 📌 Key Concepts Covered in this Lab:
* **Disaster Recovery:** Simulating a forgotten password scenario on a locked fixed data drive.
* **Alternative Authentication:** Using the "More options" UI in Windows 11 to switch from password authentication to Recovery Key authentication.
* **Key Management:** Accessing a previously backed-up `.txt` file containing the BitLocker Identifier and Recovery Key.
* **Decryption Post-Recovery:** Accessing the Control Panel to turn off BitLocker after successfully recovering access to the drive.

---

## 🖥️ Lab Scenario

* **Target Drive:** Data (D:) - Currently encrypted and **LOCKED**.
* **Problem:** You have forgotten the password (`123`) used to lock the drive.
* **Solution:** Retrieve the backup key from the **Backup (E:)** drive to unlock D:.

---

## 📋 Step-by-Step Lab Instructions

Follow these steps within the interactive simulator to complete the recovery mission:

### Part 1: Encounter the Locked Drive
1. Open **File Explorer** from the taskbar.
2. Double-click the **Locked Data (D:)** drive. The password prompt will appear.
3. Since you forgot the password, click **More options** at the bottom of the prompt.
4. Click **Enter recovery key** to switch the authentication mode.

### Part 2: Retrieve the Recovery Key
1. Leave the prompt open and navigate to the **Backup (E:)** drive using the left sidebar in File Explorer.
2. Double-click the text file named **BitLocker Recovery Key 4F8A29.txt** to open it in Notepad.
3. Highlight the 48-digit Recovery Key at the bottom of the document and click **Copy Key to Clipboard**.
4. The key will automatically paste into the BitLocker unlock prompt. Click **Unlock**.

### Part 3: Manage and Disable BitLocker
1. The drive is now unlocked (🔓)! Right-click the **Data (D:)** drive and select **Manage BitLocker**.
2. The Control Panel will open, showing the full suite of BitLocker settings.
3. Click **Turn off BitLocker** at the bottom of the options list.
4. Confirm your choice by clicking **Turn off BitLocker** in the dialog box. The drive will begin decrypting.

---

## 💻 Interactive Lab

Test your disaster recovery skills in the interactive simulation below:

[**Click Here to Access Lab 13**](https://tibinjohn193-blip.github.io/windows-11/lab13.html)
