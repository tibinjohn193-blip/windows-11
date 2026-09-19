
# Lab 12: Windows 11 BitLocker Encryption & Password Unlock

This interactive lab demonstrates how to secure a local drive using **BitLocker Drive Encryption** in Windows 11. You will learn how to enable BitLocker with a password, safely back up your recovery key, lock the drive by signing out, and unlock it again using your password. Finally, you will explore the full BitLocker management options in the Control Panel and decrypt the drive.

## 🛡️ What is BitLocker?

BitLocker is a full-volume encryption feature included with Microsoft Windows designed to protect data by providing encryption for entire volumes. It ensures that data remains secure even if a device is lost, stolen, or improperly decommissioned.

### 📌 Key Concepts Covered in this Lab:
* **Password Authentication:** Securing a fixed data drive using a strong password.
* **Recovery Key Backup:** Saving a 48-digit recovery key to an alternate drive (never the one being encrypted) to prevent permanent data loss.
* **Encryption Modes:** Choosing between "Used disk space only" (for new drives) and "New encryption mode" (XTS-AES for fixed drives).
* **Drive Locking Mechanism:** Understanding that BitLocker drives remain unlocked for the current session and require a system restart or sign-out to lock securely.
* **BitLocker Management:** Accessing the Control Panel to change passwords, remove passwords, or completely turn off BitLocker (decryption).

---

## 🖥️ Lab Scenario

* **Target Drive:** Data (D:) - This is the drive we will encrypt.
* **Backup Location:** Backup (E:) - This is where we will safely store the recovery key file.
* **Unlock Method:** Standard Password (`123`).

---

## 📋 Step-by-Step Lab Instructions

Follow these steps within the interactive simulator to complete the lab:

### Part 1: Enable BitLocker & Save Recovery Key
1. Open **File Explorer** to view your system drives.
2. Right-click on **Data (D:)** and select **Turn on BitLocker**.
3. In the BitLocker Wizard, check **Use a password to unlock the drive**, enter your password in both fields, and click Next.
4. Choose **Save to a file** to back up your recovery key.
5. In the Save dialog, select the **Backup (E:)** drive and click Save.
6. Select **Encrypt used disk space only** and click Next.
7. Select **New encryption mode** (best for fixed drives) and click Next.
8. Click **Start encrypting** and wait for the progress bar to complete. 

### Part 2: Lock the Drive
*(Note: A BitLocker drive remains unlocked after initial encryption until the system is restarted or the user signs out).*
1. Click the **Start Menu**.
2. Click your **Administrator profile** icon at the bottom left and select **Sign out**.
3. At the Windows Lock Screen, click **Sign in** to log back into the system.

### Part 3: Unlock via Password
1. Open **File Explorer**. You will now see that Data (D:) has a **Locked Padlock (🔒)** icon.
2. Double-click the locked **Data (D:)** drive.
3. A BitLocker prompt will appear in the top right corner. Enter your password and click **Unlock**. 
4. The drive icon will change to an **Unlocked Padlock (🔓)**, indicating you have access.

### Part 4: Manage and Turn Off BitLocker
1. Right-click the unlocked **Data (D:)** drive and select **Manage BitLocker**.
2. The Control Panel will open, displaying the full suite of BitLocker management options (Change password, Remove password, Back up your recovery key, etc.).
3. Click **Turn off BitLocker**.
4. Confirm by clicking **Turn off BitLocker** on the prompt. The drive will begin decrypting.

---

## 💻 Interactive Lab

Test out your skills and run through the exact configuration steps in the interactive simulation below:

[**Click Here to Access Lab 12**](https://tibinjohn193-blip.github.io/windows-11/lab12.html)
