---
title: WSL Folder in Windows
description: How to Access your Windows Subsystem Linux directory from the Windows Side
header: WSL (Windows Subsystem Linux) Folder in Windows
---

Use standard Windows networking paths to view your Linux folders using Windows Explorer.  In the search box, enter:

```
  \\wsl$
```

That will bring you to the root directory of your Linux install.  To get to your home directory, try something like this, with your version of Linux.

```
  \\wsl$\Ubuntu-18.04\home\
```

Use Visual Studio Code if you want an editor that works wonderfully with WSL.  Click on the icon on the bottom left corner to connect to your Linux install.

### references

[https://docs.microsoft.com/en-us/windows/wsl/install-win10](https://docs.microsoft.com/en-us/windows/wsl/install-win10)

#### Windows Subsystem Linux runs under Insider Build for Windows 10.