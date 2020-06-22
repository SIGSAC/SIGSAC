# Outline
### This is my exploration into Kali Linux. Join me and become elite.

### Table of Contents
1. [Installation](#Installation)
2. [Fundamentals](#Fundamentals)
3. [What is Markdown?](#Markdown-in-a-nutshell)

# Installation
Download [Kali Linux 64-Bit](https://www.kali.org/downloads/)\
Install Guest Operating System [Kali Official Guide](https://www.kali.org/docs/base-images/kali-linux-hard-disk-install/)\
Install VMWare Tools [VMWare Official Guide](http://partnerweb.vmware.com/GOSIG/Ubuntu_18_04_LTS.html)

### Specs

### Setup
1. Create a new Virtual Machine w/ Typical configurations![width=300, height=250](Kali/KaliSetup1.png)\
2. Import the downloaded Kali .iso![width=300, height=250](Kali/KaliSetup2.png)
3. Use the Linux Guest Operating System![width=300, height=250](Kali/KaliSetup3.png)
4. Give the VM a name of your choice![width=300, height=250](Kali/KaliSetup4.png)
5. Set the Disk Size![width=300, height=250](Kali/KaliSetup5.png)
6. Create the Virtual Machine![width=300, height=250](Kali/KaliSetup6.png)
6. Advanced Settings - I am using the default settings. May be liable to change in the future![width=300, height=250](Kali/KaliSetup6a.png)
7. This is a reminder that I will need to install the Kali OS, and also VMWare Tools![width=300, height=250](Kali/KaliSetup7.png)
8. Begin Kali Installation. I will be using the CLI as opposed to the GUI because it is a good practice to get comfortable with installing CLI operating systems such as Ubuntu Server Live or ApacheLinux. However, you can do a Graphical Install and the following steps will remain the same. Alternatively, the [Kali Official Guide](https://www.kali.org/docs/base-images/kali-linux-hard-disk-install/) actually runs through a GUI installation![width=300, height=250](Kali/KaliSetup8.png)
9. English![width=300, height=250](Kali/KaliSetup9.png)
10. United States![width=300, height=250](Kali/KaliSetup10.png)
12. Domain Name Optional![width=300, height=250](Kali/KaliSetup13.png)
13. Set Username![width=300, height=250](Kali/KaliSetup14.png)
14. Set Password![width=300, height=250](Kali/KaliSetup15.png)
15. Confirm Password![width=300, height=250](Kali/KaliSetup16.png)
16. Select Time Zone![width=300, height=250](Kali/KaliSetup17.png)
17. Choose Partition Disk. I chose an [Logical Volume (LVM) partition disk](https://askubuntu.com/questions/3596/what-is-lvm-and-what-is-it-used-for). LVM is very OS-experimenation-friendly and because this is the first time I am using Kali, I may change the specs of the system a lot in the future![width=300, height=250](Kali/KaliSetup18.png)
18. Select SCIS33![width=300, height=250](Kali/KaliSetup19.png)
19. All files in one partition![width=300, height=250](Kali/KaliSetup21.png)
20. Write changes to disk![width=300, height=250](Kali/KaliSetup22.png
21. (LVM Only) I maxed out the partition (20GB allocated when the VM was created). My reasoning is that likely I will be downloading a lot of tools in this Kali. If I run out of disk space, I should be able to easily increase the size because this is an LVM.![width=300, height=250](Kali/KaliSetup23.png)
22. Write changes to disk![width=300, height=250](Kali/KaliSetup24.png)
23. Did not configure HTTP proxy![width=300, height=250](Kali/KaliSetup25.png)
24. I also selected the Kali desktop environment. I'm not hardcore enough to use a CLI-only kali...yet![width=300, height=250](Kali/KaliSetup26.png)
25. Install the [GRUB boot loader](https://askubuntu.com/questions/347203/what-exactly-is-grub)![width=300, height=250](Kali/KaliSetup27.png)
26. Install boot loader on /dev/sda![width=300, height=250](Kali/KaliSetup28.png)
27. Restart the system![width=300, height=250](Kali/KaliSetup29.png)
28. Select normal bootup![width=300, height=250](Kali/KaliSetup31.png)
29. Login![width=300, height=250](Kali/KaliSetup32.png)
30. Nice, I just got Kali (Freaking awesome UI!)![width=300, height=250](Kali/KaliSetup33.png)
31. Don't forget to take a snapshot. Always take snapshots![width=300, height=250](Kali/KaliSetup34.png)