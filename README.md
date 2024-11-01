# Patched NVIDIA 372.70 INF Files for Pascal-based GPUs for use in Windows NT 6.0 (Vista/Server 2008)
This repository contains patched INF files for Windows NT 6.0 (Vista/Server 2008) for NVIDIA's Desktop 372.70 driver.

## Credits
- NVIDIA for providing drivers and INF files.
- [Me](https://github.com/eflanili7881) for patching INF files.
- Microsoft Corporation for providing various .NET Framework versions and Windows updates.
- archive.org for providing Wayback Machine service.
- User [Windows 2000](https://msfn.org/board/profile/415779-windows-2000/) from msfn.org for inspiring me to do this mod at [this thread](https://msfn.org/board/topic/177059-nvidia-pascal-graphics-card-issue/).

## What's that patch contains?
This patch contains support for probably all GPU's from v391.35 as I took all driver ID's from this version and I injected into v372.70 and it's the last version for 32-bit architecture. But I only tested this patch with NVIDIA GeForce GTX 1050 Ti as it's only non-native GPU for Windows Vista on my hand. This patch doesn't enable GPU acceleration on DirectX applications, although you can play 4K videos on MPC-HC. And this patch can only be installed on Windows NT 6.0-based OS' (Windows Vista/Server 2008) as I removed every entries for other OS'. I tested 64-bit one but I didn't tested the 32-bit one.

Don't copyright strike me, daddy NVIDIA.

## Screenshots
Here's some screenshots that I took on 2019:

![IMG_20190206_201115](https://github.com/osmankovan123/NVIDIA372.70PatchedINFsForVista/assets/44976117/f5fe7c50-58bb-4f99-8554-d647471247c3)
![IMG_20190206_211026](https://github.com/osmankovan123/NVIDIA372.70PatchedINFsForVista/assets/44976117/19617d9a-b74d-44ff-a207-5e3468848583)
![IMG_20190206_213331](https://github.com/osmankovan123/NVIDIA372.70PatchedINFsForVista/assets/44976117/1aaa45f2-2c58-47d9-bf3c-f67751cd9dc4)

## How to install this patch?
So, here's how you install this patch. But before you install this driver, I strongly suggest you to update to SP2.
- You need to install these programs and updates (Not necassary but they're improving compatibility.):
  - .NET Framework (Vanilla driver requires .NET Framework) (Select one of them, but my suggestion is download the latest version for Windows Vista)
    - .NET Framework 4.6.2 (SHA2-only signed version, Windows Server 2008 SP2 only)
      | Link | Wayback Machine mirror |
      | :-: | :-: |
      | https://dotnet.microsoft.com/en-us/ | https://web.archive.org/web/20240608084951/https://dotnet.microsoft.com/en-us/ |
      | https://dotnet.microsoft.com/en-us/download | https://web.archive.org/web/20240608085003/https://dotnet.microsoft.com/en-us/download |
      | https://dotnet.microsoft.com/en-us/download/dotnet-framework | https://web.archive.org/web/20240608085113/https://dotnet.microsoft.com/en-us/download/dotnet-framework |
      | https://dotnet.microsoft.com/en-us/download/dotnet-framework/net462 | https://web.archive.org/web/20240608084903/https://dotnet.microsoft.com/en-us/download/dotnet-framework/net462 |
      | https://dotnet.microsoft.com/en-us/download/dotnet-framework/thank-you/net462-offline-installer | https://web.archive.org/web/20240608085107/https://dotnet.microsoft.com/en-us/download/dotnet-framework/thank-you/net462-offline-installer |
      | https://go.microsoft.com/fwlink/?linkid=2099468 | https://web.archive.org/web/20240608085642/https://go.microsoft.com/fwlink/?linkid=2099468 |
      | https://download.visualstudio.microsoft.com/download/pr/8e396c75-4d0d-41d3-aea8-848babc2736a/80b431456d8866ebe053eb8b81a168b3/ndp462-kb3151800-x86-x64-allos-enu.exe | https://web.archive.org/web/20240608085546/https://download.visualstudio.microsoft.com/download/pr/8e396c75-4d0d-41d3-aea8-848babc2736a/80b431456d8866ebe053eb8b81a168b3/ndp462-kb3151800-x86-x64-allos-enu.exe |
      - But if you installed SHA2 Update on Windows Vista, you can try install .NET Framework 4.6.2 on Windows Vista SP2.
      
      | Link | Wayback Machine mirror |
      | :-: | :-: | 
      | https://support.microsoft.com/en-us/topic/the-net-framework-4-6-2-offline-installer-for-windows-9dce3874-a9e5-9b11-289d-5594824aafe0 | https://web.archive.org/web/20240608090111/https://support.microsoft.com/en-us/topic/the-net-framework-4-6-2-offline-installer-for-windows-9dce3874-a9e5-9b11-289d-5594824aafe0 |
      | http://go.microsoft.com/fwlink/?linkid=780600 | https://web.archive.org/web/20240608090507/http://go.microsoft.com/fwlink/?linkid=780600 |
      | https://download.visualstudio.microsoft.com/download/pr/8e396c75-4d0d-41d3-aea8-848babc2736a/80b431456d8866ebe053eb8b81a168b3/ndp462-kb3151800-x86-x64-allos-enu.exe | https://web.archive.org/web/20240608085546/https://download.visualstudio.microsoft.com/download/pr/8e396c75-4d0d-41d3-aea8-848babc2736a/80b431456d8866ebe053eb8b81a168b3/ndp462-kb3151800-x86-x64-allos-enu.exe |
      - Page says minimum version is Windows 7 SP1, but final out link is same as above. Therefore, it's compatible with Windows Server 2008 SP2.
      
      | Link | Wayback Machine mirror |
      | :-: | :-: | 
      | https://devblogs.microsoft.com/dotnet/announcing-net-framework-4-6-2/ | https://web.archive.org/web/20240608091831/https://devblogs.microsoft.com/dotnet/announcing-net-framework-4-6-2/ |
      | http://go.microsoft.com/fwlink/?LinkId=780601 | https://web.archive.org/web/20240608092228/http://go.microsoft.com/fwlink/?LinkId=780601 |
      | https://download.visualstudio.microsoft.com/download/pr/8e396c75-4d0d-41d3-aea8-848babc2736a/80b431456d8866ebe053eb8b81a168b3/ndp462-kb3151800-x86-x64-allos-enu.exe | https://web.archive.org/web/20240608085546/https://download.visualstudio.microsoft.com/download/pr/8e396c75-4d0d-41d3-aea8-848babc2736a/80b431456d8866ebe053eb8b81a168b3/ndp462-kb3151800-x86-x64-allos-enu.exe |
    - .NET Framework 4.6.1 (last version /wo Windows Update support before 4.6.2 was only signed with SHA-2)
      | Link | Wayback Machine mirror |
      | :-: | :-: |
      | https://dotnet.microsoft.com/en-us/ | https://web.archive.org/web/20240608084951/https://dotnet.microsoft.com/en-us/ |
      | https://dotnet.microsoft.com/en-us/download | https://web.archive.org/web/20240608085003/https://dotnet.microsoft.com/en-us/download |
      | https://dotnet.microsoft.com/en-us/download/dotnet-framework | https://web.archive.org/web/20240608085113/https://dotnet.microsoft.com/en-us/download/dotnet-framework |
      | https://dotnet.microsoft.com/en-us/download/dotnet-framework/net461 | https://web.archive.org/web/20240518114733/https://dotnet.microsoft.com/en-us/download/dotnet-framework/net461 |
      | https://dotnet.microsoft.com/en-us/download/dotnet-framework/thank-you/net461-offline-installer | https://web.archive.org/web/20240518114815/https://dotnet.microsoft.com/en-us/download/dotnet-framework/thank-you/net461-offline-installer
      | https://go.microsoft.com/fwlink/?LinkId=2099467 | https://web.archive.org/web/20240518115300/https://go.microsoft.com/fwlink/?LinkId=2099467 |
      | https://download.microsoft.com/download/E/4/1/E4173890-A24A-4936-9FC9-AF930FE3FA40/NDP461-KB3102436-x86-x64-AllOS-ENU.exe | https://web.archive.org/web/20240518115510/https://download.microsoft.com/download/E/4/1/E4173890-A24A-4936-9FC9-AF930FE3FA40/NDP461-KB3102436-x86-x64-AllOS-ENU.exe |
    - .NET Framework 4.6 (last version /w Windows Update support)
      | Link | Wayback Machine mirror |
      | :-: | :-: |
      | https://dotnet.microsoft.com/en-us/ | https://web.archive.org/web/20240608084951/https://dotnet.microsoft.com/en-us/ |
      | https://dotnet.microsoft.com/en-us/download | https://web.archive.org/web/20240608085003/https://dotnet.microsoft.com/en-us/download |
      | https://dotnet.microsoft.com/en-us/download/dotnet-framework | https://web.archive.org/web/20240608085113/https://dotnet.microsoft.com/en-us/download/dotnet-framework |
      | https://dotnet.microsoft.com/en-us/download/dotnet-framework/net46 | https://web.archive.org/web/20240518191933/https://dotnet.microsoft.com/en-us/download/dotnet-framework/net46 |
      | https://dotnet.microsoft.com/en-us/download/dotnet-framework/thank-you/net46-offline-installer | https://web.archive.org/web/20240518192126/https://dotnet.microsoft.com/en-us/download/dotnet-framework/thank-you/net46-offline-installer |
      | https://go.microsoft.com/fwlink/?LinkId=2099384 | https://web.archive.org/web/20240518192348/https://go.microsoft.com/fwlink/?LinkId=2099384 |
      | https://download.microsoft.com/download/6/F/9/6F9673B1-87D1-46C4-BF04-95F24C3EB9DA/enu_netfx/NDP46-KB3045557-x86-x64-AllOS-ENU_exe/NDP46-KB3045557-x86-x64-AllOS-ENU.exe | https://web.archive.org/web/20240518192534/https://download.microsoft.com/download/6/F/9/6F9673B1-87D1-46C4-BF04-95F24C3EB9DA/enu_netfx/NDP46-KB3045557-x86-x64-AllOS-ENU_exe/NDP46-KB3045557-x86-x64-AllOS-ENU.exe |
    - .NET Framework 4.0 Full (Client + Extended) (version that comes with v372.70 driver)
      | Link | Wayback Machine mirror |
      | :-: | :-: |
      | https://dotnet.microsoft.com/en-us/ | https://web.archive.org/web/20240608084951/https://dotnet.microsoft.com/en-us/ |
      | https://dotnet.microsoft.com/en-us/download | https://web.archive.org/web/20240608085003/https://dotnet.microsoft.com/en-us/download |
      | https://dotnet.microsoft.com/en-us/download/dotnet-framework | https://web.archive.org/web/20240608085113/https://dotnet.microsoft.com/en-us/download/dotnet-framework |
      | https://dotnet.microsoft.com/en-us/download/dotnet-framework/net40 | https://web.archive.org/web/20240518192020/https://dotnet.microsoft.com/en-us/download/dotnet-framework/net40 |
      | https://dotnet.microsoft.com/en-us/download/dotnet-framework/thank-you/net40-offline-installer | https://web.archive.org/web/20240518193308/https://dotnet.microsoft.com/en-us/download/dotnet-framework/thank-you/net40-offline-installer |
      | https://download.microsoft.com/download/9/5/A/95A9616B-7A37-4AF6-BC36-D6EA96C8DAAE/dotNetFx40_Full_x86_x64.exe | https://web.archive.org/web/20240518193521/https://download.microsoft.com/download/9/5/A/95A9616B-7A37-4AF6-BC36-D6EA96C8DAAE/dotNetFx40_Full_x86_x64.exe |
  - Platform Update (KB971644, contains 4 updates)
    - For 32-bit and 64-bit
      - https://archive.org/details/kb971644 (thanks to user [@אור הושמנד](https://archive.org/details/@user_10645) on archive.org for upload.)
    - KB960362 (Windows Ribbon and Animation Manager Library)
      - For 32-bit
        | Link | Wayback Machine mirror |
        | :-: | :-: | 
        | https://www.catalog.update.microsoft.com/Search.aspx?q=kb960362 | https://web.archive.org/web/20240518112823/https://www.catalog.update.microsoft.com/Search.aspx?q=kb960362 |
        | https://catalog.s.download.windowsupdate.com/msdownload/update/software/updt/2009/10/windows6.0-kb960362-x86_4091ebe5666232299791f4be1bf8a3fd6467326c.msu | https://web.archive.org/web/20240518112956/https://catalog.s.download.windowsupdate.com/msdownload/update/software/updt/2009/10/windows6.0-kb960362-x86_4091ebe5666232299791f4be1bf8a3fd6467326c.msu |
      - For 64-bit
        | Link | Wayback Machine mirror |
        | :-: | :-: | 
        | https://www.catalog.update.microsoft.com/Search.aspx?q=kb960362 | https://web.archive.org/web/20240518112823/https://www.catalog.update.microsoft.com/Search.aspx?q=kb960362 |
        | https://catalog.s.download.windowsupdate.com/msdownload/update/software/updt/2009/10/windows6.0-kb960362-x64_9c78c54ee0bf67e3f18315126ce2ebdc1b884b41.msu | https://web.archive.org/web/20240518113247/https://catalog.s.download.windowsupdate.com/msdownload/update/software/updt/2009/10/windows6.0-kb960362-x64_9c78c54ee0bf67e3f18315126ce2ebdc1b884b41.msu |
    - KB971512 (Windows Graphics, Imaging, and XPS Library (with DirectX 11)) (This is most important for improving graphical compatibility; others are optional)
      - For 32-bit
        | Link | Wayback Machine mirror |
        | :-: | :-: | 
        | https://www.catalog.update.microsoft.com/search.aspx?q=kb971512 | https://web.archive.org/web/20240409101608/https://www.catalog.update.microsoft.com/search.aspx?q=kb971512 |
        | https://catalog.s.download.windowsupdate.com/msdownload/update/software/updt/2009/10/windows6.0-kb971512-x86_370c3e41e1c161ddce29676e9273e4b8bb7ba3eb.msu | https://web.archive.org/web/20231007094300/https://catalog.s.download.windowsupdate.com/msdownload/update/software/updt/2009/10/windows6.0-kb971512-x86_370c3e41e1c161ddce29676e9273e4b8bb7ba3eb.msu |
      - For 64-bit
        | Link | Wayback Machine mirror |
        | :-: | :-: | 
        | https://www.catalog.update.microsoft.com/search.aspx?q=kb971512 | https://web.archive.org/web/20240409101608/https://www.catalog.update.microsoft.com/search.aspx?q=kb971512 |
        | https://catalog.s.download.windowsupdate.com/msdownload/update/software/updt/2009/10/windows6.0-kb971512-x64_0b329b985437c6c572529e5fd0042b9d54aeaa0c.msu | https://web.archive.org/web/20231007094326/https://catalog.s.download.windowsupdate.com/msdownload/update/software/updt/2009/10/windows6.0-kb971512-x64_0b329b985437c6c572529e5fd0042b9d54aeaa0c.msu |
    - KB971513 (Windows Automation API)
      - For 32-bit
        | Link | Wayback Machine mirror |
        | :-: | :-: | 
        | https://www.catalog.update.microsoft.com/Search.aspx?q=KB971513 | https://web.archive.org/web/20240518111727/https://www.catalog.update.microsoft.com/Search.aspx?q=KB971513 |
        | https://catalog.s.download.windowsupdate.com/msdownload/update/software/updt/2009/10/windows6.0-kb971513-x86_aa536aabb57dcbf2645673579512a6282a67f755.msu | https://web.archive.org/web/20240518111911/https://catalog.s.download.windowsupdate.com/msdownload/update/software/updt/2009/10/windows6.0-kb971513-x86_aa536aabb57dcbf2645673579512a6282a67f755.msu |
      - For 64-bit
        | Link | Wayback Machine mirror |
        | :-: | :-: | 
        | https://www.catalog.update.microsoft.com/Search.aspx?q=KB971513 | https://web.archive.org/web/20240518111727/https://www.catalog.update.microsoft.com/Search.aspx?q=KB971513 |
        | https://catalog.s.download.windowsupdate.com/msdownload/update/software/updt/2009/10/windows6.0-kb971513-x64_f6311b532be449d689dee8741d0a3217417bca1a.msu | https://web.archive.org/web/20240518112106/https://catalog.s.download.windowsupdate.com/msdownload/update/software/updt/2009/10/windows6.0-kb971513-x64_f6311b532be449d689dee8741d0a3217417bca1a.msu |
    - KB971514 (Windows Portable Devices Platform)
      - For 32-bit
        | Link | Wayback Machine mirror |
        | :-: | :-: | 
        | https://www.catalog.update.microsoft.com/Search.aspx?q=KB971514 | https://web.archive.org/web/20240518112244/https://www.catalog.update.microsoft.com/Search.aspx?q=KB971514 |
        | https://catalog.s.download.windowsupdate.com/msdownload/update/software/updt/2009/10/windows6.0-kb971514-x86_ae398183114294aaedfdfa950c012b3e9c99e1be.msu | https://web.archive.org/web/20240518112428/https://catalog.s.download.windowsupdate.com/msdownload/update/software/updt/2009/10/windows6.0-kb971514-x86_ae398183114294aaedfdfa950c012b3e9c99e1be.msu |
      - For 64-bit
        | Link | Wayback Machine mirror |
        | :-: | :-: | 
        | https://www.catalog.update.microsoft.com/Search.aspx?q=KB971514 | https://web.archive.org/web/20240518112244/https://www.catalog.update.microsoft.com/Search.aspx?q=KB971514 |
        | https://catalog.s.download.windowsupdate.com/msdownload/update/software/updt/2009/10/windows6.0-kb971514-x64_80986bdc1d81c6930f6387e378abebd987ce4c70.msu | https://web.archive.org/web/20240518112620/https://catalog.s.download.windowsupdate.com/msdownload/update/software/updt/2009/10/windows6.0-kb971514-x64_80986bdc1d81c6930f6387e378abebd987ce4c70.msu |
  - Platform Update Supplement (KB2117917)
    - For 32-bit
      | Link | Wayback Machine mirror |
      | :-: | :-: | 
      | https://www.catalog.update.microsoft.com/Search.aspx?q=kb2117917 | https://web.archive.org/web/20240518113435/https://www.catalog.update.microsoft.com/Search.aspx?q=kb2117917 |
      | https://catalog.s.download.windowsupdate.com/msdownload/update/software/updt/2011/02/windows6.0-kb2117917-x86_370435d9efa6643c44d6506666b1960d56cf673a.msu | https://web.archive.org/web/20240518113606/https://catalog.s.download.windowsupdate.com/msdownload/update/software/updt/2011/02/windows6.0-kb2117917-x86_370435d9efa6643c44d6506666b1960d56cf673a.msu |
    - For 64-bit
      | Link | Wayback Machine mirror |
      | :-: | :-: | 
      | https://www.catalog.update.microsoft.com/Search.aspx?q=kb2117917 | https://web.archive.org/web/20240518113435/https://www.catalog.update.microsoft.com/Search.aspx?q=kb2117917 |
      | https://catalog.s.download.windowsupdate.com/msdownload/update/software/updt/2011/02/windows6.0-kb2117917-x64_655a21758801e9648702791d7bf30f81b58884b3.msu | https://web.archive.org/web/20240518113757/https://catalog.s.download.windowsupdate.com/msdownload/update/software/updt/2011/02/windows6.0-kb2117917-x64_655a21758801e9648702791d7bf30f81b58884b3.msu |
  - Windows Driver Framework version 1.11 update (KB2761494) (This is most important for improving driver compatibility.)
    - For 32-bit
      | Link | Wayback Machine mirror |
      | :-: | :-: | 
      | https://www.catalog.update.microsoft.com/Search.aspx?q=KB2761494 | https://web.archive.org/web/20240518113942/https://www.catalog.update.microsoft.com/Search.aspx?q=KB2761494 |
      | https://catalog.s.download.windowsupdate.com/msdownload/update/software/updt/2012/12/windows6.0-kb2761494-x86-mergedpkg_d1a88e28183646281d95cd8150bdd09faa0d2a9e.msu | https://web.archive.org/web/20240518114207/https://catalog.s.download.windowsupdate.com/msdownload/update/software/updt/2012/12/windows6.0-kb2761494-x86-mergedpkg_d1a88e28183646281d95cd8150bdd09faa0d2a9e.msu |
    - For 64-bit
      | Link | Wayback Machine mirror |
      | :-: | :-: | 
      | https://www.catalog.update.microsoft.com/Search.aspx?q=KB2761494 | https://web.archive.org/web/20240518113942/https://www.catalog.update.microsoft.com/Search.aspx?q=KB2761494 |
      | https://catalog.s.download.windowsupdate.com/msdownload/update/software/updt/2012/12/windows6.0-kb2761494-x64-mergedpkg_4f986add28318ed72dc950c89b0d1ef80e8d4319.msu | https://web.archive.org/web/20240518114339/https://catalog.s.download.windowsupdate.com/msdownload/update/software/updt/2012/12/windows6.0-kb2761494-x64-mergedpkg_4f986add28318ed72dc950c89b0d1ef80e8d4319.msu |
- Download NVIDIA GeForce Game Ready Driver version 372.70 for Windows 7, 8 and 8.1 with corresponding architecture.
  - Starting with v340.52?, driver packages still splitted to desktop and notebook prefixes, but these packages hashes are same:
    | Desktop 32-bit | Notebook 32-bit |
    | :-: | :-: |
    | ![image](https://github.com/osmankovan123/NVIDIA372.70PatchedINFsForWinNT6.0/assets/44976117/3ee83aca-38fb-4ce1-8731-96f63b17a604) | ![image](https://github.com/osmankovan123/NVIDIA372.70PatchedINFsForWinNT6.0/assets/44976117/5dfa2278-a71f-4e4a-b016-6cc54130c503) |
    - For Desktop 32-bit:
      | Link | Wayback Machine mirror |
      | :-: | :-: | 
      | https://www.nvidia.com/download/driverResults.aspx/107007/en-us/ | https://web.archive.org/web/20240517200045/https://www.nvidia.com/download/driverResults.aspx/107007/en-us/ |
      | https://www.nvidia.com/content/DriverDownloads/confirmation.php?url=/Windows/372.70/372.70-desktop-win8-win7-32bit-international-whql.exe&lang=us&type=GeForce | https://web.archive.org/web/20240517200124/https://www.nvidia.com/content/DriverDownloads/confirmation.php?url=/Windows/372.70/372.70-desktop-win8-win7-32bit-international-whql.exe&lang=us&type=GeForce |
      | https://us.download.nvidia.com/Windows/372.70/372.70-desktop-win8-win7-32bit-international-whql.exe | https://web.archive.org/web/20240517194936/https://us.download.nvidia.com/Windows/372.70/372.70-desktop-win8-win7-32bit-international-whql.exe |
    - For Desktop 64-bit:
      | Link | Wayback Machine mirror |
      | :-: | :-: | 
      | https://www.nvidia.com/download/driverResults.aspx/107008/en-us/ | https://web.archive.org/web/20240517195744/https://www.nvidia.com/download/driverResults.aspx/107008/en-us/ |
      | https://www.nvidia.com/content/DriverDownloads/confirmation.php?url=/Windows/372.70/372.70-desktop-win8-win7-64bit-international-whql.exe&lang=us&type=GeForce | https://web.archive.org/web/20240517195902/https://www.nvidia.com/content/DriverDownloads/confirmation.php?url=/Windows/372.70/372.70-desktop-win8-win7-64bit-international-whql.exe&lang=us&type=GeForce |
      | https://us.download.nvidia.com/Windows/372.70/372.70-desktop-win8-win7-64bit-international-whql.exe | https://web.archive.org/web/20240517194120/https://us.download.nvidia.com/Windows/372.70/372.70-desktop-win8-win7-64bit-international-whql.exe |
    - For Notebook 32-bit
      | Link | Wayback Machine mirror |
      | :-: | :-: | 
      | https://www.nvidia.com/download/driverResults.aspx/107009/en-us/ | https://web.archive.org/web/20240518173442/https://www.nvidia.com/download/driverResults.aspx/107009/en-us/ |
      | https://www.nvidia.com/content/DriverDownloads/confirmation.php?url=/Windows/372.70/372.70-notebook-win8-win7-32bit-international-whql.exe&lang=us&type=geforcem | https://web.archive.org/web/20240518173646/https://www.nvidia.com/content/DriverDownloads/confirmation.php?url=/Windows/372.70/372.70-notebook-win8-win7-32bit-international-whql.exe&lang=us&type=geforcem |
      | https://us.download.nvidia.com/Windows/372.70/372.70-notebook-win8-win7-32bit-international-whql.exe | https://web.archive.org/web/20240518173853/https://us.download.nvidia.com/Windows/372.70/372.70-notebook-win8-win7-32bit-international-whql.exe |
    - For Notebook 64-bit
      | Link | Wayback Machine mirror |
      | :-: | :-: | 
      | https://www.nvidia.com/download/driverResults.aspx/107010/en-us/ | https://web.archive.org/web/20240518175038/https://www.nvidia.com/download/driverResults.aspx/107010/en-us/ |
      | https://www.nvidia.com/content/DriverDownloads/confirmation.php?url=/Windows/372.70/372.70-notebook-win8-win7-64bit-international-whql.exe&lang=us&type=geforcem | https://web.archive.org/web/20240518175201/https://www.nvidia.com/content/DriverDownloads/confirmation.php?url=/Windows/372.70/372.70-notebook-win8-win7-64bit-international-whql.exe&lang=us&type=geforcem |
      | https://us.download.nvidia.com/Windows/372.70/372.70-notebook-win8-win7-64bit-international-whql.exe | https://web.archive.org/web/20240518175329/https://us.download.nvidia.com/Windows/372.70/372.70-notebook-win8-win7-64bit-international-whql.exe |
- Extract driver package via archive manager.
  - You can use 7-Zip or other archiving software that has ability to expanding SFX archives.
- Copy Display.Driver folder corresponding your architecture to the extracted driver folder. Replace any files.
- Double-click setup.exe to start installation.
- On driver installation, select Custom.
- Untick nView from install (Cannot start in Vista/Server 2008 in vanilla anyway; it may work with Extended Kernel).
- Start installation by clicking Next.
- After installation is complete, reboot PC. If installation successful, resolution should be increased to the native resolution.
  - The screen maybe don't come for up to 30 seconds or longer on first boot. After that, system will start normally on other boots.
