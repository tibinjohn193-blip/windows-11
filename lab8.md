
# Lab 8: Windows 11 Local User Management (`lusrmgr.msc`)

This interactive lab demonstrates how to manage local user accounts and groups in Windows 11 using the Local Users and Groups management console. You will learn how to create users, manage passwords, control account access, and escalate privileges.

## 📖 What is Local User Management?

Windows allows multiple people to share the same computer by creating separate user accounts. The **Local Users and Groups (`lusrmgr.msc`)** console is an advanced administrative tool used by IT professionals to centrally manage these accounts, control their status, and assign them to specific security groups (like the Administrators group).

## 🎯 Lab Objectives

*   Access the Local Users and Groups console via the Windows Run dialog.
*   Create a new local user account and set an initial password.
*   Navigate the Windows login screen to switch between user profiles.
*   Force a password reset for a standard user from an administrative account.
*   Disable and re-enable access to a user account.
*   Grant administrative privileges to a standard user by adding them to the Administrators security group.

---

## 📋 Step-by-Step Lab Instructions

Follow these steps within the simulator to complete the lab:

### Part 1: Create a New User
1. **Open the Console:** Click the **Start Menu (🪟)**, search for `run`, and open the Run app. Type `lusrmgr.msc` and click **OK**.
2. **Navigate to Users:** Click on the **Users** folder in the left sidebar.
3. **Create Account:** Right-click an empty space in the center pane and select **New User...**
4. **Set Details:** Enter a username (e.g., `User1`) and a password. Uncheck "User must change password at next logon", click **Create**, and then close the dialog.

### Part 2: Test the New Account
1. **Switch User:** Click the **Start Menu (🪟)**, click the **Administrator** profile picture at the bottom left, and select **Switch user / Sign out**.
2. **Log In:** On the lock screen, select your newly created user, enter the password, and click **Submit**. 
3. **Return to Admin:** Once logged in, open the Start Menu again, click the user profile, and switch back to the **Administrator** account.

### Part 3: Reset Password & Disable Account
1. **Reopen Console:** Use Run (`Win + R`) to open `lusrmgr.msc` again.
2. **Reset Password:** Right-click your new user and select **Set Password...**. Acknowledge the warning, enter a new password, and save.
3. **Disable Account:** Double-click the user to open their Properties. Check the **Account is disabled** box and click **Apply**. Notice the downward red arrow icon appear over the user. *(Uncheck it and click Apply again to re-enable the account for the next step).*

### Part 4: Grant Administrator Privileges
1. **Access Member Tab:** Inside the user's Properties window, click the **Member Of** tab at the top.
2. **Add Group:** Click the **Add...** button.
3. **Assign Role:** In the object names box, type `Administrators` and click **OK**.
4. **Finalize:** Click **OK** on the Properties window to save your changes. The user now has full administrative rights on the PC.

---

## 💻 Interactive Lab

Test out your skills and run through the exact configuration steps in the interactive simulation below:

[**Click Here to Access Lab 8**](https://tibinjohn193-blip.github.io/windows-11/lab8.html)
