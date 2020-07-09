<link rel="stylesheet" type="text/css" href="Computers 101.css">

# Computers 101
## *Learn the fundamentals of computers and Operating Systems*

## Table of Contents
1. [Boot Process](#Boot-Process)
2. [Terminology](#Terminology)
3. [Resources and links used](#Resources-and-links-used)

## Boot Process
<figure>
  <img src="assets/Computers 101/Linux-Boot-Process.png" alt="my alt text"/>
  <figcaption>Figure 1. Boot Process</figcaption>
</figure>

### Phase 1: [BIOS/System Start](#BIOS)
1. BIOS conducts [POST](#POST) test to check hardware is working. Background process you won't see.
2. Looks for an [MBR](#MBR) or [GPT](#GPT) to determine what OS is loaded and from where to boot. Background process you won't see.
### Phase 2: [MBR loading & GRUB Bootloader](#Bootloader)
3. The MBR runs the bootloader which loads the rest of the [OS](#OS). Linux typically uses GRUB
### Phase 3: [Kernel](#Kernel)
4. The kernel is the first program that is loaded after the bootloader. The kernel remains in memory and handles all low-level tasks between hardware and user such as disk management, memory management, task management, and more. 
### Phase 4: [INIT Process](#INIT)
5. The init program initializes the system in the required way. Think of wildfire, once you have a fire started you can spread the fire. Without an initial fire started, the fire cannot be spread. The init process maintains the process of starting the system and shutting it down.
### Phase 5: User Prompt
6. The user prompt is the final level of the boot process. This is the terminal or CMD prompt that you see and can interact with. In modern OS's, this is known as the GUI (graphical user interface), providing a safe and easy method of interacting with the computer.

[Video Explanation](https://www.youtube.com/watch?v=mHB0Z-HUauo)

## Terminology

### Boot
* To turn on. Comes from the word "[bootstrap](https://en.wiktionary.org/wiki/pull_oneself_up_by_one%27s_bootstraps)" which is the process by which a computer pulls itself from a dead state into a fully functioning machine

### Bootloader
* Code that loads the OS

### BIOS
**Basic Input Output System**
* Firmware (Software that provides low level control over device hardware) First program to run which kickstarts the boot process

### GPT
**GUID Partition Table**
* New standard replacing MBR, usually 512 byte section that contains the bootloader information.

### GRUB
**GRand Unified Bootloader**
* First software that starts at system boot; GRUB loads the Linux kernel

### INIT
* Process with process ID 1, started by the kernel, and resists signal 9 (kills processes). All other programs are either started by init or by its child processes.

### initrd
**"initial ramdisk"**
* The first 

### Kernel
* Responsible for low-level tasks such as disk management, memory management, task management, etc
* Allows for interface between user and system components

### MBR
**Master Boot Record**
* 512 byte section of the first sector on a disk that contains the bootloader information.
* MBR only works with disks up to 2 TB in size.

### Partition
* Section of storage device, treated as a separate logical volume. 
* Emulates a separate physical device.

### POST
**Power-on self-test**
* Process run by BIOS to check hardware like memory, disk drives and that it works properly.

### **ROM**
**Read-only memory**
* As name implies. Little to no [volatility](#volatility)

### **RAM**
**Random Access Memory**
* When a program runs, it performs a lot of mathematical calculations to move bits around. RAM provides an area to store all those bits.
* Older machines had 2-4GB RAM. Cadet laptops have 32GB RAM
* RAM does not have persistence, a reboot or loss of power WILL cause the RAM to lose all content.
* High [volatility](#volatility)

### **CPU**
**Central Processing Unit**
* The brain of the computer. 
* Proccesses input, stores data, and outputs results
* Basically a hodge-podge of circuits, logic gates, and transistors

### **Volatility**
* How easily/quickly it changes


### **OS**
**Operating System**
* System software that manages computer hardware, software, and more. Ones you may be familiar with:

| Windows | Linux | MacOS | 
| - | - | - |
| Windows XP | Ubuntu | High Sierra |
| Windows 7 | CentOS | Mojave |
| Windows 10 | Kali | Catalina |


### HDD
**Hard Drive Disk**
* Platter - The disk as a whole
* Track - A single ring on the platter (Red Ring)
* (Geometrical) Sector - Looks like the mathematical version of a sector (Blue Portion)
* Track Sector - Smallest accessible unit on disk (Intersection of Blue & Red)
* Cluster - Group of track sectors (Green Portion)

<figure>
  <img src="assets/Computers 101/Hard Disk.jpg" alt="A visual description of how a Hard Drive Disk operates"/>
  <figcaption>Figure 1. Boot Process</figcaption>
</figure>

### Solid State Disk
<figure>
<img src="assets/Computers 101/HDDvsSSD.png" alt="A visual comparision of a Hard Disk Drive vs a Solid State Drive"/>
<figcaption>Figure 3. HDD vs SSD</figcaption>

[Linux Boot Process](https://www.youtube.com/watch?v=mHB0Z-HUauo)

[GRUB boot loader](https://askubuntu.com/questions/347203/what-exactly-is-grub)

## How to dual boot (DO NOT DO THIS ON YOUR CADET LAPTOP)
***DO NOT DO THIS TO YOUR CADET LAPTOP***
- Boot from an ubuntu usb in live mode
- Using the Ubuntu's built in partition tool, unmount Normal ubnutu machine from the computer.
- If the ubuntu machine is using the full machine, resize the ubuntu machine to use only half.
- Power off the machine
- Plug in the usb containing the second image you want to dual boot
- THe windows boot loader will show you all the unallocated space available for you to use.
- Go through the remaining OS download process
- Fix your boot loader to accomodate for two machines


## Resources and links used

https://www.howtogeek.com/193669/whats-the-difference-between-gpt-and-mbr-when-partitioning-a-drive/

https://www.khanacademy.org/computing/computers-and-internet#xcae6f4a7ff015e7d:computers

https://afteracademy.com/blog/what-is-kernel-in-operating-system-and-what-are-the-various-types-of-kernel

https://www.pks.mpg.de/~mueller/docs/suse10.2/html/opensuse-manual_en/manual/sec.boot.init.html