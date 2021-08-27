# InstallWSL2Guide

**Reference**<br>
[Windows Subsystem for Linux Installation Guide for Windows 10](https://docs.microsoft.com/en-us/windows/wsl/install-win10#manual-installation-steps)

## Manual Installation Steps

**Step 1 - Enable the Windows Subsystem for Linux**<br>

Open PowerShell as **Administrator** and run:<br>
```postscript
PS C:\> dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
```
![Image](https://github.com/neolin-ms/InstallWSL2Guide/pics/blob/main/2021-08-26_163947.png)

**Step 2 - Check requirements for running WSL 2**<br>
To update to WSL 2, you must be running Windows 10.

* For x64 systems: Version 1903 or higher, with Build 18362 or higher.
* For ARM64 systems: Version 2004 or higher, with Build 19041 or higher.

**Step 3 - Enable Virtual Machine feature**<br>
**Step 4 - Download the Linux kernel update package**<br>
**Step 5 - Set WSL 2 as your default version**<br>
**Step 6 - Install your Linux distribution of choice**<br>

