# Guide for creating an Ubuntu 20.04 VM
This guide will use VirtualBox. I am very sorry M1 users :( this is not a guide for you.

## Starting Off
1. Install VirtualBox. You can find the packages [here](https://www.virtualbox.org/wiki/Downloads). If you are on a Linux distribution, you can also install Virtual Box through your distro's software installation system if you so choose.
2. Download the Ubuntu 20.04 ISO image [here](https://ubuntu.com/download/desktop). This is freee!!!!. click to download the desktop image (you may download the server image if you know what you are doing, this guide will not assist with that).

## Creating the Virtual Machine
1. Open VirtualBox and click the '**New'** button. You can give your VM a name, and then choose '**Linux'** for '**Type'** and select '**Ubuntu (64 bit)'** in the '**Version'** drop down menu.
2. On the next screen, set the ammount of **memory (RAM)** for your machine (atleast 2GB of RAM, I allocated 4GB). **DO NOT ALLOCATE MORE MEMORY THAN YOUR HOST MACHINE HAS.**
3. On the next screen, leave the option '**Create a virtual hard disk now'** set and hit the '**Create'** button. On the following screen, leave the option '**VDI (VirtualBox Disk Image)'** set and press the '**Continue'** button. On the next screen, leave the '**Dynamically allocated'** option set, and press the '**Continue'** button.
4. You will now be prompted to select a size for the virtual disk (I chose a size of 24GB). Then press the '**Create'** button.
5. Now, select your newly created VM and click '**Settings'**, then go to '**Storage'** and select the '**Empty'** optical drive under '**Controller: IDE'**. Click the disk icon on the right of the window, and click '**Choose Virtual Optical Disk File'**.
6. Click '**add'** and select the ISO image of Ubuntu that you dowloaded earlier.

## Getting Started with Ubuntu
1. Select your VM and hit '**Start'**. This will boot up the Ubuntu installation system.
2. Once it's ready, click '**Install Ubuntu'**. Then, select your keyboard layout.
3. On the next screen, you can select '**Normal Installation'** or '**Minimal Installation'**. I recommend the minimal installation, as it takes up less space. Once you have selected, click the '**Continue'** button.
4. The next screen will ask you whether you would like to '**Erase disk and install Ubuntu'** or do '**Something else'**. Select '**Erase disk and install Ubuntu'**. Do not fret, this will only affect the virtual hard disk. Next, select '**Install Now'**. A pop up will show up, press '**Continue'**.
5. On the next screen, select your timezone, and then setupt your user account. Press '**Continue'**, and wait for the installation to finish. When it's done, click '**Restart'**. Follow the instructions from there.

## Packages
Useful packages for this class:
* build-essentials
* clang
* gcc
* make
* clang-format
* git
* valgrind
* gdb

You may install all of these using the follwing command:\
`sudo apt install build-essentials clang gcc make clang-format git valgrind gdb`\
You may also benefit from installing VirtualBox guest additions:\
`sudo apt install virtualbox-guest-utils virtualbox-guest-x11 virtualbox-guest-dkms`\
You will need to restart your machine right after this, per the installation instructions.
