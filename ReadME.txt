+-----------------------------------------+NVIDIA Pascal Support For Windows Vista/2008+-----------------------------------------+
I Hi, and thanks for downloading my patch for Windows Vista. How I required this patch is I need Windows Vista on GTX 1050 Ti    I
I on bare-metal machine (VM's are obsolete here.). So, I did a research for this subject and I prepared this patch for you.      I
I                                                                                                                                I
I So, here's how you install this patch:                                                                                         I
I 0)You need to install these updates (Not necassary but they're improving compatibiliy.):                                       I
I   -.NET Framework 4.6.1                                                                                                        I
I   -Platform Update (KB971644, contains 4 updates)                                                                              I
I    -KB971512 = Windows Graphics, Imaging, and XPS Library (with DirectX 11) (At least, this is required; others are optional)  I
I    -KB971513 = Windows Automation API                                                                                          I
I    -KB971514 = Windows Portable Devices Platform                                                                               I
I    -KB960362 = Windows Ribbon and Animation Manager Library                                                                    I
I   -Platform Update Supplement (KB2117917)                                                                                      I
I   -Windows Driver Framework version 1.11 update (KB2761494)                                                                    I
I 1)Download NVIDIA Windows 7 372.70 with corresponding architecture.                                                            I
I 2)Extract this archive via archive manager.                                                                                    I
I 3)Copy Display.Driver folder corresponding your architecture to the extracted driver folder. Replace any files.                I
I 4)Double-click setup.exe to start installation.                                                                                I
I 5)On driver installation, select Custom.                                                                                       I
I 6)Untick nView from install (Cannot start in Vista; it may work with Extended Kernel).                                         I
I 7)Start installation by clicking Next.                                                                                         I
I 8)After Setup is complete, reboot PC. If installation successful, resolution should be increased to the native resolution.     I
+--------------------------------------------------------------------------------------------------------------------------------+