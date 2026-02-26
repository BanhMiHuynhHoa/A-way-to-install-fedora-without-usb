# A-way-to-install-fedora-without-usb
## Pre-installation
Things you will need
* Your favorite fedora image
* A partition management tool. you can use the "create and format ..." on windows

Steps
1. Create a FAT32 partition for storing the image and name it, i will name it LINUXBOOT

![](partition.png)  
2. Mount your image, turn on view hidden files, copy all of it to the LINUXBOOT  
3. On the LINUXBOOT partition, go to boot\grub2 and edit the grub.cfg file  
4. Find the section "menuentry "Start Fedora-Workstation-Live"" or the first menuentry section that you see  
5. At the CD label, change it to your partition name, amd at the end of that line, add rd.live.ram=1, this will make you boot the installer on your ram, it should look like this  
![]()
6. Now restart and boot on that partition you have
