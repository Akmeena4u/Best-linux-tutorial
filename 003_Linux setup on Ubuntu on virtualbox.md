### Installing Ubuntu on VirtualBox
Select a Linux distribution based on your needs (e.g., Ubuntu, Fedora, Debian, CentOS, etc.). Here we have selected Ubuntu

VirtualBox enables you to create virtual machines where Ubuntu (or other Linux distributions) can be installed and used for various purposes such as development, testing, education, and system administration, all within a virtualized and isolated environment on your host machine.

**Step 1: Download Ubuntu ISO**
- Visit the Official Ubuntu Website and download the ISO file for Ubuntu. [Official site](https://ubuntu.com/download/desktop)
  ![image](https://github.com/Akmeena4u/Best-linux-tutorial/assets/93425334/01ba7491-dc33-4e28-8524-f20cd91b9733)


**Step 2: Open VirtualBox**
- Launch VirtualBox on your computer. [VirtualBox](https://www.geeksforgeeks.org/how-to-install-virtualbox-in-linux/)
   ![image](https://github.com/Akmeena4u/Best-linux-tutorial/assets/93425334/5857e4ab-44fb-45a0-970b-909e2412d172)

  
**Step 3: Create a New Virtual Machine**
- Click on the "New" button in VirtualBox to create a new virtual machine.
- Enter a name for your virtual machine and choose the type and version (Ubuntu, 64-bit).
  ![image](https://github.com/Akmeena4u/Best-linux-tutorial/assets/93425334/3a3859dd-8a92-4714-a8fa-5996f973546f)

**Step 4: Assign RAM and Create Virtual Hard Disk**
- Allocate RAM size for your virtual machine (e.g., 2GB is sufficient for basic use).
- Create a virtual hard disk by selecting "Create a virtual hard disk now."
  ![image](https://github.com/Akmeena4u/Best-linux-tutorial/assets/93425334/81ac8de1-6a36-4824-a076-ee437c00f82a)


**Step 5: Choose Hard Disk Settings**
- Select the type of hard disk (VDI is recommended).
- Choose between dynamically allocated or fixed size storage (dynamically allocated is recommended).
  ![image](https://github.com/Akmeena4u/Best-linux-tutorial/assets/93425334/ac60436b-eb36-48e7-9063-7d08d5c21065)


**Step 6: Set Disk Size and Location**
- Specify the disk size (e.g., 20GB for Ubuntu).
- Choose the destination folder where the virtual machine will be installed.
  ![image](https://github.com/Akmeena4u/Best-linux-tutorial/assets/93425334/25ad302e-9afe-41b9-8dae-8a2539410ec9)


**Step 7: Boot the Virtual Machine**
- Start the virtual machine you just created in VirtualBox.

**Step 8: Install Ubuntu**
- If the installation disk is not automatically detected, browse and select the Ubuntu ISO file you downloaded.
- Follow the on-screen instructions to install Ubuntu on the virtual machine.
  ![image](https://github.com/Akmeena4u/Best-linux-tutorial/assets/93425334/45d3290e-0958-43fb-bc22-56860ef2c2f4)


**Step 9: Configure Installation Settings**
- Choose language, keyboard layout, and installation type (e.g., Normal Installation is recommended).
- Create a user account and set up your preferences.

**Step 10: Complete Installation**
- Click on "Install Now" to start the installation process.
- Follow the prompts and provide necessary information during the installation.

**Step 11: Post-Installation Setup**
- Set your time zone and location.
- Choose a name for your computer and set a password for user login.

**Step 12: Finalize Installation**
- Wait for the installation process to complete.
- Once done, reboot your virtual machine.

**Step 13: Make Full Screen**
- To make Ubuntu fullscreen in VirtualBox, insert Guest Additions CD Image by clicking on Devices > Insert Guest Additions CD Image.
- Open Terminal and run the commands:
  ```
  sudo apt update
  sudo apt upgrade
  ```
- Execute the Guest Additions installation script by running:
  ```
  ./autorun.sh
  ```
- Restart Ubuntu to enable full-screen mode.

### FAQs

**How to install Ubuntu on VirtualBox?**
1. Download Ubuntu ISO.
2. Open VirtualBox, create a new VM, assign RAM and create a virtual hard disk.
3. Boot VM, select Ubuntu ISO, and follow on-screen instructions to install.

**How to install VirtualBox?**
1. Visit the VirtualBox official page.
2. Download the executable file.
3. Run the installer and follow on-screen instructions to install VirtualBox.

**Is installing Ubuntu on VirtualBox different from normal disk installation?**
Yes, installing Ubuntu on VirtualBox is simpler as you don't need to create new disk partitions like in a normal disk installation.
