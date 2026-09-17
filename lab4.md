# Windows System Restore Lab Guide

**System Restore** is a Windows recovery tool designed to fix issues by reverting your computer's software and settings back to a previous, working state. It works by taking a "snapshot" (called a Restore Point) of your core system files, Windows Registry, and installed programs at a specific moment in time.

## 🛠️ Primary Uses

*   **Undoing Bad Updates:** If a new Windows update or hardware driver causes your computer to crash or run poorly, System Restore rolls back those changes.
*   **Removing Problematic Software:** If a recently installed application corrupts your system settings or causes instability, reverting to a restore point undoes the installation.
*   **Fixing Unexplained Errors:** When your system starts behaving erratically and you cannot pinpoint the cause, jumping back to a date when everything worked is often the fastest fix.

> **⚠️ Important Note:** System Restore only affects system files, installed applications, and registry settings. It is completely safe for your personal data—it will not delete, alter, or recover your personal documents, photos, videos, or emails.

---

## 📋 Step-by-Step Restoration Process

Follow this sequence to perform a System Restore (based on the lab simulation):

### 1. Access the Recovery Environment
*   **Action:** From the Windows interface, hold down the `Shift` key on your keyboard, click the **Power** icon, and select **Restart**. Continue holding `Shift` until the system reboots.
*   **Verification:** Your computer will boot into a blue screen titled "Choose an option" instead of your normal desktop.

### 2. Navigate to System Restore
*   **Action:** On the blue WinRE screen, click **Troubleshoot**, then click **Advanced options**, and finally select **System Restore**.
*   **Verification:** The screen will prompt you to choose an account to continue.

### 3. Authenticate Your Account
*   **Action:** Click on your administrator account name (e.g., "admin"), enter your password(in our system 123 is the password ), and click **Continue**.
*   **Verification:** The classic white "System Restore" wizard window will open on your screen.

### 4. Select the Restore Point
*   **Action:** Click **Next** on the welcome screen. Click on the specific restore point you want to use (such as your manual "smec" point) to highlight it in blue, then click **Next**.
*   **Verification:** You chose the correct one if the date, time, and description match your target on the final "Confirm your restore point" screen.

### 5. Start the Restoration
*   **Action:** Click **Finish**, and then click **Yes** on the final warning popup (the process cannot be interrupted).
*   **Verification:** A progress bar will appear showing initialization and file restoration, followed by an automatic system restart.

---

## 💻 Interactive Lab

[**Click Here to Access the Lab Simulation**](https://tibinjohn193-blip.github.io/windows-11/LAB%204%20restore%20os%20using%20ytem%20restore%20point%20%20.html)
