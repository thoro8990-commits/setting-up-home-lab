# setting-up-home-lab
Setting up a homelab involves building a personal computing environment to experiment with hardware, networking, virtualization, and self-hosted software.
Phase 1: Download & Install VMware Workstation Pro
(Note: Broadcom offers VMware Workstation Pro for free for personal use.)
Sign in or register for a free account.
Under Software > VMware Cloud Foundation > My Downloads, search for VMware Workstation Pro.
Download the installer for your host operating system (Windows or Linux).
![Image Alt](https://github.com/thoro8990-commits/setting-up-home-lab/blob/8e36133a7df60c0bd9821f436fcb7049b190f583/Screenshot%202026-10-06%20132140.png)
Phase 2: Install VMware:
Open the downloaded setup file (e.g., .exe on Windows).
Follow the installation wizard (default options are recommended).
Complete the wizard and restart your computer if prompted.
![Image Alt](https://github.com/thoro8990-commits/setting-up-home-lab/blob/ade5a096d994f40df994d0f32fb04fa7b59cc67b/image.png)
Phase 3: Download Kali Linux
Go to the official Kali Linux download page: kali.org/get-kali
Pick the (Fastest & Easiest): Pre-built Virtual Machine Image, is easier to configure 
Select the Virtual Machines option.
Download the VMware 64-bit pre-built image (.7z file).
![Image Alt](https://github.com/thoro8990-commits/setting-up-home-lab/blob/39e21432abceb21ce62c6a928399d17e6ef6a7a1/Screenshot%202026-10-06%20202749.png)
Phase 3: Setting Up Kali Linux in VMware
Method A: Using the Pre-built VMware Image (Recommended)
Extract the file: Right-click the downloaded .7z file and extract it using 7-Zip or WinRAR.
Open in VMware:
Launch VMware Workstation Pro.
Click File > Open... (or click Open a Virtual Machine).
Navigate to the extracted folder and select the .vmx configuration file.
Boot up:
Click Power on this virtual machine. Pick the image file downloaded 
![Image Alt](https://github.com/thoro8990-commits/setting-up-home-lab/blob/325484becf796e834a074e95cc481c15169ff2e9/Screenshot%202026-10-06%20203341.png)
Select Installer disc image file (ISO), click Browse, and select your downloaded Kali Linux .iso file. Click Next.
Choose Linux. In the version dropdown, choose Debian 12.x 64-bit (or Other Linux 6.x kernel 64-bit).
Configure VM Settings:
VM Name: Set to Kali Linux, Disk Size: Allocate at least 40 GB – 80 GB.
Choose Store virtual disk as a single file.
Hardware Allocation: Memory (RAM): Assign at least 2 GB to 4 GB (4 GB / 4096 MB recommended). Processors: Assign at least 2 TO 4 CPU cores.
Network Adapter: Set to NAT (shares host internet) or Bridged (gives VM its own IP on the local network). Click Close, then Finish.
Power on the Virtual Machine.
![Image Alt](https://github.com/thoro8990-commits/setting-up-home-lab/blob/0771b8af873fbc108f32904a2f8cfbf53193dad2/Screenshot%202026-10-06%20203504.png)
At the boot menu, select Graphical Install.
Select your Language, Country/Location, and Keyboard Layout. Hostname & Domain: Set hostname (default kali) and leave domain blank.
User Creation: Create a new username and a strong password. Partitioning: Choose Guided - use entire disk, select the virtual disk, and pick All files in one partition.
Confirm write changes to disk by selecting Yes.
Software Selection: Leave default desktop environment (Xfce) and tool selections checked, then click Continue.
GRUB Boot Loader: When prompted, select Yes to install GRUB, choose /dev/sda as the target device, and continue.
Once finished, click Continue to reboot. Log in with the credentials created during setup.
![Image Alt](https://github.com/thoro8990-commits/setting-up-home-lab/blob/e81613e7200125a62577e4a96327699625b3e60e/Screenshot%202026-10-06%20204819.png )
Phrase 4: Then it will finally take you to the login page where you put your default password kali/kali, then it open the kali home page, after that click terminal and input your first command "sudo apt update && upgrade", to make your kali linux up to date
![Image Alt](https://github.com/thoro8990-commits/setting-up-home-lab/blob/2030a8a3c5e0169143de10f9980b43a88c2c42a9/Screenshot%202026-10-06%20205413.png)
