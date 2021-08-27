# InstallWSL2Guide

**Reference**<br>
* [Windows Subsystem for Linux Installation Guide for Windows 10](https://docs.microsoft.com/en-us/windows/wsl/install-win10#manual-installation-steps)
* [changes to updating the WSL2 Linux kernel](https://devblogs.microsoft.com/commandline/wsl2-will-be-generally-available-in-windows-10-version-2004)
* [Windows Command Line Blog](https://aka.ms/cliblog)

## Manual Installation Steps

**Step 1 - Enable the Windows Subsystem for Linux**<br>

Open PowerShell as **Administrator** and run:<br>
```postscript
PS C:\> dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
```

![Image](https://github.com/neolin-ms/InstallWSL2Guide/pics/blob/main/2021-08-26_163947.png)

**Step 2 - Check requirements for running WSL 2**<br>

To update to WSL 2, you must be running Windows 10.<br>

* For x64 systems: Version 1903 or higher, with Build 18362 or higher.
* For ARM64 systems: Version 2004 or higher, with Build 19041 or higher.

To check your version and build number, select Windows logo key + R, type winver, select OK.<br>

![Image](https://github.com/neolin-ms/InstallWSL2Guide/pics/blob/main/2021-08-26_163947.png)

**Step 3 - Enable Virtual Machine feature**<br>

Open PowerShell as Administrator and run:<br>
```postscript
PS C:/> dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
```
**Important: Restart your machine to complete the WSL install and update to WSL 2.**

![Image](https://github.com/neolin-ms/InstallWSL2Guide/pics/blob/main/2021-08-26_163947.png)

**Step 4 - Download the Linux kernel update package**<br>

4-1 Download the latest package: [WSL2 Linux kernel update package for x64 machines](https://wslstorestorage.blob.core.windows.net/wslblob/wsl_update_x64.msi)

4-2 Run the update package downloaded in the previous step. (Double-click to run - you will be prompted for elevated permissions, select ‘yes’ to approve this installation.)

![Image](https://github.com/neolin-ms/InstallWSL2Guide/pics/blob/main/2021-08-26_163947.png)

**Step 5 - Set WSL 2 as your default version**<br>

Open PowerShell as Administrator and run this command to set WSL 2 as the default version when installing a new Linux distribution:<br>

![Image](https://github.com/neolin-ms/InstallWSL2Guide/pics/blob/main/2021-08-26_163947.png)

**Step 6 - Install your Linux distribution of choice**<br>

6-1 Open the Microsoft Store and select your favorite Linux distribution.

![Image](https://github.com/neolin-ms/InstallWSL2Guide/pics/blob/main/2021-08-26_163947.png)

6-2 From the distribution's page, select "Get".

![Image](https://github.com/neolin-ms/InstallWSL2Guide/pics/blob/main/2021-08-26_163947.png)

6-3 You will then need to create a user account and password for your new Linux distribution.

![Image](https://github.com/neolin-ms/InstallWSL2Guide/pics/blob/main/2021-08-26_163947.png)

**ONGRATULATIONS! You've successfully installed and set up a Linux distribution that is completely integrated with your Windows operating system!**


