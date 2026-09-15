SYSTEM RESTORE

System Restore is a Windows recovery tool designed to fix issues by reverting your computer's software and settings back to a previous, working state.

It works by taking a "snapshot" (called a Restore Point) of your core system files, Windows Registry, and installed programs at a specific moment in time.

Here are its primary uses:

    Undoing Bad Updates: If a new Windows update or hardware driver causes your computer to crash or run poorly, System Restore rolls back those changes.

    Removing Problematic Software: If a recently installed application corrupts your system settings or causes instability, reverting to a restore point undoes the installation.

    Fixing Unexplained Errors: When your system starts behaving erratically and you cannot pinpoint the cause, jumping back to a date when everything worked is often the fastest fix.

Important Note: System Restore only affects system files, installed applications, and registry settings. It is completely safe for your personal data—it will not delete, alter, or recover your personal documents, photos, videos, or emails


Here is the step-by-step process for performing a System Restore, following the exact sequence from your lab simulation

.1.Access the Recovery Environment:Shift + Restart.From the Windows interface, hold down the Shift key on your keyboard, click the Power icon, and select Restart. Continue holding Shift until the system reboots. 
To verify this step was successful, your computer will boot into a blue screen titled "Choose an option" instead of your normal desktop.

2.Navigate to System Restore:WinRE Menus.On the blue screen, click Troubleshoot, then click Advanced options, and finally select System Restore. You can verify you selected the correct path when the screen prompts you to choose an account to continue.

3.Authenticate Your Account:Admin Password.Click on your administrator account name (e.g., "admin"), enter your password (like "123" in your lab), and click Continue. This step is successful if the classic white "System Restore" wizard window opens on your screen.

4.Select the Restore Point:Wizard Options.Click Next on the welcome screen. Click on the specific restore point you want to use (such as your manual "smec" point) to highlight it in blue, then click Next. You can verify you chose the right one by checking the date, time, and description on the final "Confirm your restore point" screen.

5.Start the Restoration:Do not interrupt.Click Finish, and then click Yes on the final warning popup that tells you the process cannot be interrupted. To verify the restoration has successfully started, a progress bar will appear showing initialization and file restoration, followed by an automatic system restart.
