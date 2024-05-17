# Patched NVIDIA 372.70 INF Files for Pascal-based GPU for use in Windows Vista
This repository contains patched INF files for Windows Vista for NVIDIA's Desktop 372.70 driver.

## Credits
- NVIDIA for providing INF files.
- Me for patching INF files.

## What's that patch contains?
This patch contains support for probably all GPU's from v391.35 as I took all driver ID's from this version and I injected into v372.70 and it's the last version for 32-bit architecture. But I only tested this patch with NVIDIA GeForce GTX 1050 Ti as it's only non-native GPU for Windows Vista. This patch doesn't enable GPU acceleration on DirectX applications, although you can play 4K videos on MPC-HC. And this patch can only be installed on Windows NT 6.0-based OS' as I removed every entries for other OS'. I tested 64-bit one but I didn't tested the 32-bit one.

## How to install this patch?
So, here's how you install this patch.
- You need to install these updates (Not necassary but they're improving compatibility.):
  - .NET Framework 4.6.1
  - Platform Update (KB971644, contains 4 updates)
    - KB971512 (Windows Graphics, Imaging, and XPS Library (with DirectX 11)) (This is most important for improving graphical compatibility; others are optional)
    - KB971513 (Windows Automation API)
    - KB971514 (Windows Portable Devices Platform)
    - KB960362 (Windows Ribbon and Animation Manager Library)
  - Platform Update Supplement (KB2117917)
  - Windows Driver Framework version 1.11 update (KB2761494) (This is most important for improving graphical compatibility.)
- Download NVIDIA GeForce Game Ready Driver version 372.70 for Windows 7, 8 and 8.1 with corresponding architecture.
  - For 64-bit:
    - https://www.nvidia.com/download/driverResults.aspx/107008/en-us/
      - Wayback Machine mirror:
        - https://web.archive.org/web/20240517195744/https://www.nvidia.com/download/driverResults.aspx/107008/en-us/
    - https://www.nvidia.com/content/DriverDownloads/confirmation.php?url=/Windows/372.70/372.70-desktop-win8-win7-64bit-international-whql.exe&lang=us&type=GeForce
      - Wayback Machine mirror:
        - https://web.archive.org/web/20240517195902/https://www.nvidia.com/content/DriverDownloads/confirmation.php?url=/Windows/372.70/372.70-desktop-win8-win7-64bit-international-whql.exe&lang=us&type=GeForce
    - https://us.download.nvidia.com/Windows/372.70/372.70-desktop-win8-win7-64bit-international-whql.exe
      - Wayback Machine mirror:
        - https://web.archive.org/web/20240517194120/https://us.download.nvidia.com/Windows/372.70/372.70-desktop-win8-win7-64bit-international-whql.exe
  - For 32-bit:
    - https://www.nvidia.com/download/driverResults.aspx/107007/en-us/
      - Wayback Machine mirror:
        - https://web.archive.org/web/20240517200045/https://www.nvidia.com/download/driverResults.aspx/107007/en-us/
    - https://www.nvidia.com/content/DriverDownloads/confirmation.php?url=/Windows/372.70/372.70-desktop-win8-win7-32bit-international-whql.exe&lang=us&type=GeForce
      - Wayback Machine mirror:
        - https://web.archive.org/web/20240517200124/https://www.nvidia.com/content/DriverDownloads/confirmation.php?url=/Windows/372.70/372.70-desktop-win8-win7-32bit-international-whql.exe&lang=us&type=GeForce
    - https://us.download.nvidia.com/Windows/372.70/372.70-desktop-win8-win7-32bit-international-whql.exe
      - Wayback Machine mirror:
        - https://web.archive.org/web/20240517194936/https://us.download.nvidia.com/Windows/372.70/372.70-desktop-win8-win7-32bit-international-whql.exe
- Extract this archive via archive manager.
- Copy Display.Driver folder corresponding your architecture to the extracted driver folder. Replace any files.
- Double-click setup.exe to start installation.
- On driver installation, select Custom.
- Untick nView from install (Cannot start in Vista; it may work with Extended Kernel).
- Start installation by clicking Next.
- After Setup is complete, reboot PC. If installation successful, resolution should be increased to the native resolution.
