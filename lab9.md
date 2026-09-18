# Lab 9: Windows 11 User Management via Command Line (CMD)

This interactive lab demonstrates how to manage local user accounts in Windows 11 entirely through the Command Line Interface (CLI). Using the `net user` and `net localgroup` commands, you will learn how to create, modify, and delete user accounts without relying on the graphical user interface.

## 📖 What is Command-Line User Management?

While Windows provides graphical tools like `lusrmgr.msc` and the Settings app to manage users, system administrators often prefer the command line for its speed and automation capabilities. The built-in `net` command allows administrators to quickly execute user management tasks, which is especially useful when writing deployment scripts or managing servers remotely.

## 🎯 Lab Objectives

*   Launch the Command Prompt with Administrator privileges.
*   Create a new local user account with a predefined password.
*   View detailed account properties and status.
*   Reset a user's password securely.
*   Disable and re-enable a user account.
*   Elevate a standard user to the Administrators group.
*   Delete a user account from the system.

---

## 📋 Step-by-Step Lab Instructions

Follow these commands within the simulator's Administrator Command Prompt to complete the lab:

### 1. Launch Command Prompt as Administrator
*   Click the **Start Menu (🪟)**.
*   Type `cmd` in the search box.
*   On the right side of the search results, click **🛡️ Run as administrator**.

### 2. Create a New User Account
*   **Command:** `net user User1 123 /add`
*   **Action:** Creates a new local account named "User1" with the password "123".

### 3. View User Properties
*   **Command:** `net user User1`
*   **Action:** Displays the account's details, including whether the account is active and its group memberships.

### 4. Reset the User's Password
*   **Command:** `net user User1 456`
*   **Action:** Instantly changes User1's password to "456".

### 5. Disable the User Account
*   **Command:** `net user User1 /active:no`
*   **Action:** Disables the account, preventing the user from logging in.
*   *Tip: Run `net user User1` again to verify the "Account active" status now says "No".*

### 6. Re-Enable the User Account
*   **Command:** `net user User1 /active:yes`
*   **Action:** Reactivates the account.

### 7. Grant Administrator Privileges
*   **Command:** `net localgroup Administrators User1 /add`
*   **Action:** Adds User1 to the local Administrators group.
*   *Tip: Run `net user User1` to verify "*Administrators" appears under Local Group Memberships.*

### 8. Delete the User Account
*   **Command:** `net user User1 /delete`
*   **Action:** Permanently removes User1 from the system.

### 9. Verify Deletion
*   **Command:** `net user`
*   **Action:** Lists all current user accounts on the PC. Verify that User1 is no longer listed.

---

## 💻 Interactive Lab

Test out your skills and run through the exact configuration steps in the interactive simulation below:

[**Click Here to Access Lab 9**](https://tibinjohn193-blip.github.io/windows-11/lab9..html)
