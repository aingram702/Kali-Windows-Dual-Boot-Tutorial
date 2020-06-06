# Kali-Windows-Dual-Boot-Tutorial
Step-by-step guide to create a dual-boot system using Kali Linux and Windows 10.

## Requirements:
- 20 GB minimum disk space for Kali Linux installation. **However I recommend much more than that.**
- CD-DVD/USB boot support.
- Kali Linux ISO image or Windows 10 installer image. For this example I will be starting out with a Windows 10 machine. **Starting with Windows 10 installation is easiest.**
- Disk imaging software like Etcher or Win32 Disk Imager
- Non-PXE system

## Step 1) Backup data incase of failure or mistake during this process.

## Step 2) Enter your BIOS/UEFI and change boot-order to give priority to USB or CD-DVD.

## Step 3) Download and burn your desired disk image to either USB or CD-DVD:
1. Download Kali Linux Live image at [kali.org downloads page](https://www.kali.org/downloads/)
2. Open your disk imaging software and select your USB or CD-DVD. Then select your disk image and burn image to medium.

## Step 4) Create partition for Kali Linux OS. 20 GB minimum. 
1. Back up important files incase of failure.  
2. Right-click Start Icon, and select Disk Management. 
3. Locate the disk you wish to use. It will be the disk that contains your C: Drive.
4. Right-click the drive and select **Shrink Volume...**
5. Find the box labeled **Enter the amount of space to shrink in MB:** and resize to leave at least 20 GB free space.
6. Click button labeled **Shrink**.

### DO NOT format the free space. Kali installer will do that for you.

## Step 5) Install Kali-Linux.
1. Insert USB drive or CD-DVD and reboot into the Kali Linux menu.
2. Choose either **Install** or **Graphical install**.
3) Follow basic install instructions described here [Hard-disk Install](https://www.kali.org/docs/installation/kali-linux-hard-disk-install/) until you reach **Partition disks** section.
4. Choose option labeled **Guided-use the largest continuous free space**. This will create necessary partitions in the free space you created in Step 4.
5. Finish installation steps until completed. Once completed, safely remove installation medium, and reboot system. If done correctly you will be greeted with a GRUB boot menu that allows you to choose either Kali Linux or Windows 10. 
6. Enjoy your new dual-boot system. 


## NOTE:
- If you are starting out with a Kali Linux system the steps are basically the same except instead of using Windows Disk Management you will use GParted software included with Kali OS. **Also resize to leave 32 GB of free space instead of 20 GB as described above.**
