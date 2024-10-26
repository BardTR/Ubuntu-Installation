# Ubuntu 24.04 Installation Guide

This guide will walk you through the steps to install Ubuntu **24.04** on your computer. It includes instructions for downloading the ISO file, creating a bootable USB, and installing Ubuntu. Follow each step carefully to ensure a smooth installation.

## Table of Contents

* [Prerequisites](#prerequisites)
* [Step 1: Download Ubuntu 24.04 ISO](#step-1-download-ubuntu-2404-iso)
* [Step 2: Create a Bootable USB](#step-2-create-a-bootable-usb)
* [Step 3: Boot from USB](#step-3-boot-from-usb)
* [Step 4: Ubuntu Installation](#step-4-ubuntu-installation)
  * [Step 4.1: Choose Language](#step-4-ubuntu-installation)
  * [Step 4.2: Select Keyboard Layout](#step-4-ubuntu-installation)
  * [Step 4.3: Connect to Wi-Fi](#step-4-ubuntu-installation)
  * [Step 4.4: Update and Install Options](#step-4-ubuntu-installation)
  * [Step 4.5: Partitioning](#step-4-ubuntu-installation)
  * [Step 4.6: User and System Setup](#step-4-ubuntu-installation)
  * [Step 4.7: Start Installation](#step-4-ubuntu-installation)
  * [Step 4.8: Finishing Installation](#step-4-ubuntu-installation)
* [Post-Installation Setup](#post-installation-setup)
* [Troubleshooting](#troubleshooting)
* [Additional Resources](#additional-resources)

## Prerequisites

* **Computer** with at least 4GB of RAM and 25GB of available storage space.
* **USB Flash Drive** (12GB or larger) to create a bootable drive.
* **Backup** all important data from your computer before proceeding.
* **Internet Connection** for downloading updates and additional features during installation.

### Step 1: Download Ubuntu 24.04 ISO
1. Visit the official [Ubuntu](https://ubuntu.com/) download page.
2. Find and download the latest [Ubuntu 24.04 LTS](https://ubuntu.com/download/desktop/thank-you?version=24.04.1&architecture=amd64&lts=true) ISO file.
3. Save the file to a convenient location, such as your desktop.

### Step 2: Create a Bootable USB

You need to create a bootable USB from the ISO file. Use one of the following methods:

#### On Windows
* Download and install Rufus from [Rufus.ie](https://rufus.ie/en/).
* Open Rufus and select your USB drive.
* Under "Boot selection," click "Select" and choose the downloaded Ubuntu 24.04 ISO file.
* Leave the rest of the options as default and click Start.

#### On macOS
* Download and install balenaEtcher from [balena.io/etcher](https://etcher.balena.io/).
* Open balenaEtcher, select the Ubuntu 24.04 ISO, and choose your USB drive.
* Click Flash to create the bootable USB.

#### On Linux
* Open a terminal and run the following command:
* Bash
```bash        
sudo dd if=/path/to/ubuntu-24.04.iso of=/dev/sdX bs=4M status=progress
```
* Replace **/path/to/ubuntu-24.04.iso** with the path to the ISO file and **/dev/sdX** with your USB device (e.g., /dev/sdb).

### Step 3: Boot from USB

* Insert the bootable USB drive into your computer.
* Restart the computer and enter the Boot Menu (usually by pressing F12, Esc, F2, DEL, varies to [manufacturer](#some-of-the-manufacturer-bios-keys-for-examples)).
* Select the USB drive from the Boot Menu to start the Ubuntu installer.

### Step 4: Ubuntu Installation
  
  #### Step 4.1: Choose Language
 * On the welcome screen, select your preferred language and click **Continue**.
  
  #### Step 4.2: Select Keyboard Layout
 * Choose your keyboard layout and click **Continue**.
  
  #### Step 4.3: Connect to Wi-Fi
 * If prompted, select your **Wi-Fi** network and enter the password.
  
  #### Step 4.4: Update and Install Options
 * **Normal Installation**: Includes all default apps.
 * **Minimal Installation**: Only includes basic utilities and a web browser.
 * Check **Download updates while installing Ubuntu** and **Install third-party software** for graphics, Wi-Fi, etc.
  
  #### Step 4.5: Partitioning
 * **Erase disk and install Ubuntu**: Installs Ubuntu and deletes existing data on the selected drive.
 
 * **Something else**: Allows custom partitioning.
   
   * **Recommended**: Create separate partitions for root (/), home (/home), and swap.
     
     * Root (/): 20GB minimum
     * Home (/home): Remaining space
     * Swap: Equal to RAM size (recommended for systems with 4GB or less RAM)
  
  #### Step 4.6: User and System Setup
   * Enter your **name, computer name, username, and password**.
   * Choose whether you want to log in automatically or require a password at login.
  
  #### Step 4.7: Start Installation
   * Review your settings and click **Install Now** to begin the installation.
   * Follow any on-screen instructions, if applicable.
  
  #### Step 4.8: Finishing Installation
   * When installation completes, click **Restart Now** and remove the bootable USB drive when prompted.
   * Your computer will restart into **Ubuntu 24.04**.

## Post-Installation Setup

After your first boot, consider these additional steps:

1. Update the System :

``` bash
sudo apt update && sudo apt upgrade -y
```

2. Install Additional Software:

   * **Snap** and **Flatpak** provide easy access to a range of software.

   * Examples:

   ``` bash
   sudo apt install gimp vlc
   ```
3. Set Up Drivers (if applicable):
   
   * **Go to Settings > Additional Drivers** to install proprietary drivers if needed.

4. Enable Firewall:

   ```bash
   sudo ufw enable
   ```

## Troubleshooting

If you encounter any issues, here are a few tips:

* **No Bootable Device Found**: Double-check BIOS settings for boot sequence and enable UEFI/Legacy mode if required.
* **No Wi-Fi**: Try an Ethernet connection during installation, or look for third-party drivers post-installation.
* **Black Screen after Reboot**: Check display drivers in Advanced Options under the GRUB menu.

## Additional Resources
* [Official Ubuntu Documentation](https://help.ubuntu.com/)
* [Ask Ubuntu (Community Support)](https://ubuntu.com/community/support)
### Some of the manufacturer BIOS keys for examples
  * ASRock: F2 or DEL
  * ASUS: F2 for all PCs, F2 or DEL for Motherboards
  * Acer: F2 or DEL
  * Dell: F2 or F12
  * ECS: DEL
  * Gigabyte / Aorus: F2 or DEL
  * HP: F10
  * Lenovo (Consumer Laptops): F2 or Fn + F2
  * Lenovo (Desktops): F1
  * Lenovo (ThinkPads): Enter then F1.
  * MSI: DEL for motherboards and PCs
  * Microsoft Surface Tablets: Press and hold volume up button.
  * Origin PC: F2
  * Samsung: F2
  * Toshiba: F2
  * Zotac: DEL
