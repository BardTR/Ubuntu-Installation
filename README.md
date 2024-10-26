![ubuntu-logo-png-ubuntu-logo-free-logo-icons-1200x630](https://github.com/user-attachments/assets/5885df1d-dbe5-4ead-92e1-8d92c2ee9bf7)
# Ubuntu 24.04 Installation Guide

This guide will walk you through the steps to install Ubuntu **24.04** on your computer. It includes instructions for downloading the ISO file, creating a bootable USB, and installing Ubuntu. Follow each step carefully to ensure a smooth installation.

## Table of Contents

* [Recommended Minimum System Requirements](#recommended-minimum-system-requirements)
* [Step 1: Download Ubuntu 24.04 ISO](#step-1-download-ubuntu-2404-iso)
* [Step 2: Create a Bootable USB](#step-2-create-a-bootable-usb)
* [Step 3: Boot from USB](#step-3-boot-from-usb)
* [Step 4: Ubuntu Installation](#step-4-ubuntu-installation)
  * [Step 4.1: Choose Language](#step-41-choose-language)
  * [Step 4.2: Accessibility](#step-42-accessibility)
  * [Step 4.3: Select Keyboard Layout](#step-43-select-keyboard-layout)
  * [Step 4.4: Connect to Wi-Fi](#step-44-connect-to-wi-fi)
  * [Step 4.5: Update and Install Options](#step-45-update-and-install-options)
  * [Step 4.6: Partitioning](#step-46-partitioning)
  * [Step 4.7: User and System Setup](#step-47-user-and-system-setup)
  * [Step 4.8: Start Installation](#step-48-start-installation)
  * [Step 4.9: Finishing Installation](#step-49-finishing-installation)
* [Post-Installation Setup](#post-installation-setup)
* [Troubleshooting](#troubleshooting)
* [Additional Resources](#additional-resources)

## Recommended Minimum System Requirements

* 2 GHz dual-core **processor**
* 4096 MiB RAM (system memory) for **physical** installs.
* 2048 MiB RAM for **virtualised** installs.
* 25 GB (8.6 GB for minimal) of **hard-drive** space (or USB stick, memory card or external drive but see [LiveCD](https://help.ubuntu.com/community/LiveCD) for an alternative approach)
* 3D acceleration-capable **GPU** with at least 256 MB of VRAM
* 1024x768 or higher **resolution** display
* 16 GB (or larger) **USB flash drive**
* **Backup** all important data from your computer before proceeding.
* **Internet Connection** for downloading updates and additional features during installation.

### Step 1: Download Ubuntu 24.04 ISO
1. Visit the official [Ubuntu](https://ubuntu.com/) download page.
2. Find and download the latest [Ubuntu 24.04 LTS](https://ubuntu.com/download/desktop/thank-you?version=24.04.1&architecture=amd64&lts=true) ISO file.
3. Save the file to a convenient location, such as your desktop.

![Screenshot_9](https://github.com/user-attachments/assets/e621b135-1dea-458c-8f45-4ed9c5972c12)

### Step 2: Create a Bootable USB

You need to create a bootable USB from the ISO file. Use one of the following methods:

#### On Windows
* Download and install Rufus from [Rufus.ie](https://rufus.ie/en/).
* Open Rufus and select your USB drive.
* Under "Boot selection," click "Select" and choose the downloaded Ubuntu 24.04 ISO file.
* Leave the rest of the options as default and click Start.

![Screenshot_12](https://github.com/user-attachments/assets/41090d18-9816-4aad-95f3-c8a8256a9238)

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
    * *OR* Use Windows 11 or 10's Advanced Start Menu to access BIOS 

![Screenshot_1](https://github.com/user-attachments/assets/9986628b-82fb-4b86-b03d-7041189a1225)

![EpVCmtiii6EuWS7gv8ASe4-970-80](https://github.com/user-attachments/assets/a3e1ec32-f4be-4ed4-9414-0f758b746d1e)

![25E6MBcC5oQhX5BFGcmB4D-970-80](https://github.com/user-attachments/assets/2cf38c1b-7373-4735-aec9-e5b0436cca33)

![8Kd4LQAUDP9Ju4aqJMZu3J-970-80](https://github.com/user-attachments/assets/9e953ed3-4000-4b42-83ae-9e96858fc654)

![7JpAUvMefEPo58HwKZLFQf-970-80](https://github.com/user-attachments/assets/0222acff-995d-4e0a-99d2-dd029aed42a0)

* Select the USB drive from the Boot Menu to start the Ubuntu installer.

![Screenshot_15](https://github.com/user-attachments/assets/d07417ce-32da-446a-8388-1c05998451b6)

![Screenshot_16](https://github.com/user-attachments/assets/25f63d50-9bc1-41f0-8aec-e72e43da53ce)

![Screenshot_1](https://github.com/user-attachments/assets/fb1acc0d-af55-4a6b-97c3-90f97f1e2b25)

### Step 4: Ubuntu Installation
  
  #### Step 4.1: Choose Language
 * On the welcome screen, select your preferred language and click **Next**.
  
![Screenshot_1](https://github.com/user-attachments/assets/653ca945-97a0-464c-9223-946218750d5b)

  #### Step 4.2: Accessibility
  * If you need accessibility features, select them and click **Next**
![Screenshot_3](https://github.com/user-attachments/assets/36d95bc9-973a-4080-98d4-023a7566224a)
  
![Screenshot_4](https://github.com/user-attachments/assets/8e597e2d-dcd5-4b3d-8150-36021a7c5560)

![Screenshot_5](https://github.com/user-attachments/assets/1349caf1-d5b4-4730-b613-188408f1d1f6)

![Screenshot_6](https://github.com/user-attachments/assets/574b710e-7c6c-4b79-b814-dc517b8d6494)

![Screenshot_7](https://github.com/user-attachments/assets/79a4fc4f-f74e-4cda-8974-f2c269f6a6b7)


  #### Step 4.3: Select Keyboard Layout
 * Choose your keyboard layout and click **Next**.
  
![Screenshot_8](https://github.com/user-attachments/assets/403d347e-a646-4acb-8542-1271774af011)

  #### Step 4.4: Connect to Wi-Fi
 * If prompted, select your **Wi-Fi** network and enter the password.

![Screenshot from 2024-10-26 09-59-38](https://github.com/user-attachments/assets/cc73e5bb-16b0-432d-a3b6-bcb6e9501ad9)

![Screenshot from 2024-10-26 10-00-16](https://github.com/user-attachments/assets/1c38485a-4943-4517-8842-08561d989931)

  #### Step 4.5: Update and Install Options
 * **Default Installation**: Only includes basic utilities and a web browser.
 * **Extended Installation**: Includes all apps.
 * Check **Download updates while installing Ubuntu** and **Install third-party software** for graphics, Wi-Fi, etc.

![Screenshot_10](https://github.com/user-attachments/assets/a49d0025-d5dd-40fc-8381-f03c1e1b94f0)

![Screenshot_11](https://github.com/user-attachments/assets/256d79d3-1c30-4206-b299-9e9d5956abc3)

![Screenshot from 2024-10-26 09-59-17](https://github.com/user-attachments/assets/de497121-c649-40f2-9251-c7a44e63e16d)


  #### Step 4.6: Partitioning
 
 * **Installs Ubuntu alongside Windows Boot Manager**: Installs Ubuntu with Windows.
 
 * **Erase disk and install Ubuntu**: Installs Ubuntu and deletes existing data on the selected drive.
 
 ![Screenshot from 2024-10-26 10-05-32](https://github.com/user-attachments/assets/d7f45ad4-98b7-4327-ab00-3e68cb009a4a)

 ![Screenshot from 2024-10-26 10-05-04](https://github.com/user-attachments/assets/771e02be-939e-4bd1-a608-e21cfb6642ed)


 * **Manual Installation**: Create separate partitions for root (/), home (/home), and swap.
     
   * Root (/): 20GB minimum
   * Home (/home): Remaining space
   * Swap: Equal to RAM size (recommended for systems with 4GB or less RAM)
  
  #### Step 4.7: User and System Setup
   * Enter your **name, computer name, username, and password**.
   * Choose whether you want to log in automatically or require a password at login.
  
![Screenshot_13](https://github.com/user-attachments/assets/1d86c6dd-f4c4-436e-b9f2-1a8bf47a5a13)

![Screenshot_14](https://github.com/user-attachments/assets/74993048-76ae-4ee9-842c-9990d34a9312)


  #### Step 4.8: Start Installation
   * Review your settings and click **Install Now** to begin the installation.
   * Follow any on-screen instructions, if applicable.
  
  #### Step 4.9: Finishing Installation
   * When installation completes, click **Restart Now** and remove the bootable USB drive when prompted.
   * Your computer will restart into **Ubuntu 24.04**.

## Post-Installation Setup (Optional)

After your first boot, consider these additional steps:

1. Update the System :

Bash
``` bash
sudo apt update && sudo apt upgrade -y
```

2. Install Additional Software:

   * **Snap** and/or **Flatpak** provide easy access to a range of software.

   * Examples: *installs VLC media player*
   
   Bash
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
