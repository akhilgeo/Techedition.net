---
title: Format a USB drive using command prompt
layout: post
author: sal
categories:
- Jekyll
- tutorial
image: assets/images/16.jpg
---

Formatting a USB drive is a useful way to erase its contents and prepare it for a new use. While there are many third-party tools available to format USB drives, you can also format a USB drive through Command Prompt on a Windows computer. In this blog post, we will guide you through the steps to format USB through Command Prompt.

Step 1: Connect the USB Drive

First, connect the USB drive to your Windows computer. Make sure the drive is properly connected and detected by the system.

Step 2: Open Command Prompt

Next, open Command Prompt on your Windows computer. You can do this by pressing the Windows key + R to open the Run dialog box, typing "cmd" and hitting Enter.

Step 3: Select the USB Drive

Once Command Prompt is open, type "diskpart" and press Enter. This will open the DiskPart command-line utility. Type "list disk" and press Enter to see the list of all available disks on your computer, including the USB drive. Identify the number associated with the USB drive you want to format.

Step 4: Select the USB Drive

Type "select disk [disk number]" and press Enter. Replace [disk number] with the number associated with the USB drive you want to format. This command will select the USB drive for formatting.

Step 5: Clean the USB Drive

Type "clean" and press Enter. This command will remove all partitions and data on the selected USB drive.

Step 6: Create a New Partition

Type "create partition primary" and press Enter. This command will create a new primary partition on the selected USB drive.

Step 7: Format the USB Drive

Type "format fs=ntfs quick" and press Enter. This command will format the USB drive with the NTFS file system. You can replace "ntfs" with "fat32" or "exfat" if you prefer those file systems. The "quick" parameter will perform a quick format, which is faster than a full format.

Step 8: Assign a Drive Letter

Type "assign letter=[drive letter]" and press Enter. Replace [drive letter] with the drive letter you want to assign to the USB drive. This will make the USB drive accessible in File Explorer.

Step 9: Exit DiskPart

Type "exit" and press Enter to exit the DiskPart command-line utility.

Conclusion

Formatting a USB drive through Command Prompt can be a quick and easy way to prepare the drive for a new use. By following these simple steps, you can format your USB drive with ease. However, it's essential to be cautious while using DiskPart, as it can also erase the data on your hard drive if used incorrectly. Therefore, it's recommended to double-check the disk number before proceeding with the formatting process.
