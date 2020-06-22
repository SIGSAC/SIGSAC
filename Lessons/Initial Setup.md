# Outline
### You've received your team laptop. Here is what you should do:
 
1. [Laptop Setup](#Laptop-Setup)
2. [Github Setup](#Github-Setup)
3. [Practice](#Practice)
   
# Laptop Setup

Reboot your computer and hit `F12` as it is booting up. Select the medium you want to install from (San Disk). 
Install Ubuntu with the following:

1. Open your laptop and click Install Ubuntu![width=300, height=250](pictures/setup1.png)
   
2. Select English![width=300, height=250](pictures/setup2.png)
   
3. Select English(US)![width=300, height=250](pictures/setup3.png)
   
4. Minimal Installation w/ updates & third-party software![width=300, height=250](pictures/setup4.png)
   
5. Erase Disk and Install Ubuntu![width=300, height=250](pictures/setup5.png)
   
6. Continue (if the following screen popsup)![width=300, height=250](pictures/setup5a.png)
   
7. New York![width=300, height=250](pictures/setup6.png)
   
8. Customize your computer![width=300, height=250](pictures/setup7.png)
   
9.  Wait for Installation![width=300, height=250](pictures/setup8.png)
    
10. Restart computer![width=300, height=250](pictures/setup9.png)


# Github Setup
Once you have a clean Ubuntu 18.04 image, set up your GitHub:

>### Github in a nutshell
>Github lets you collaborate on files with other people. 
>1. First, you need access to a repository (*a special folder that is both hosted on GitHub servers and also downloaded to your local machine*)
>2. Next, you can edit the code file on your computer with a text editor (Notepad, Sublime, Atom, Vim, Visual Studio etc)
>3. After, you will **add** the file a queue, **commit** those changes (make sure to add a comment), and then **push** them from the queue to GitHub's servers.


Update BASH and install git
```
sudo apt update && sudo apt install git
```
![width=300, height=250](pictures/Github1.png)

Generate a public-private key pair.
```
ssh-keygen -t ed25519 -a 256
```
![width=300, height=250](pictures/Github2.png)

### Access the "BORG" repository
1. Print the public key
```
git clone git@github.com:bitsforeveryone/borg
```
![width=300, height=250](pictures/Github3.png)

2. Login to GitHub![width=300, height=250](pictures/Github4.png)
   
3. Go to Settings![width=300, height=250](pictures/Github5.png)
   
4. Configure SSH & GPG keys![width=300, height=250](pictures/Github6.png)
   
5. Paste public key![width=300, height=250](pictures/Github7.png)
   
6. Clone Team repository(BORG)
```
git clone git@github.com:bitsforeveryone/borg
```
![width=300, height=250](pictures/Github8.png)

## Download Team Tools
1. Run script to download Team tools
```
./borg/infra/laptops/c3t.sh
```
![width=300, height=250](pictures/Github9.png)

2. Allow all users to run Wireshark ![width=300, height=250](pictures/WiresharkSetup.png)
   
3. VMWare Workstation 15.5 Pro Setup
   1. Accept Terms![width=300, height=250](pictures/VMWareSetup2.png)

   3. Allow Updates![width=300, height=250](pictures/VMWareSetup3.png)

   4. Your Choice![width=300, height=250](pictures/VMWareSetup4.png)

   5. Automatic![width=300, height=250](pictures/VMWareSetup5.png)

   6. Automatic![width=300, height=250](pictures/VMWareSetup6.png)

   7. Use Port 443![width=300, height=250](pictures/VMWareSetup7.png)

   8. Enter Confirmation Key: `44284-XZJ05-N8VD4-0A0H6-28VPJ`![width=300, height=250](pictures/VMWareSetup8.png)