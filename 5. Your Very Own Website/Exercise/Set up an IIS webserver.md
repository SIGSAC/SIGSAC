# Setting up a webpage in Windows Internet Information Services (IIS)

*Written and tested by yours truly, [43y3s](https://github.com/incub4t0r)*

## **Table of Contents**

1. [Installing IIS](#Installing-IIS)
    1. [Checking installation](#Checking-installation)
2. [Creating our first website](#Creating-our-first-website)
    1. [Pre-reqs](#Pre-reqs)
    2. [Making the site](#Making-the-site)
3. [Troubleshooting](#Troubleshooting)
4. [Uninstalling IIS](#Uninstalling-IIS)

## **Installing IIS**

1.  Hit the windows key and start typing `Turn Windows` and select `Turn Windows features on or off`.
2.  Scroll to find `Internet Information Services`.
3.  Check the box to filled, and ensure that everything except FTP is filled as well.


<p align="center"><img src="assets/images/windowsfeatures.png" height="400"></p>


4.  Press OK, and reboot computer.

### **Checking installation**

Open a browser tab, and navigate to `http://localhost` in the search bar, and you should be met with a blue webpage shown below.


<p align="center"><img src="assets/images/iisstart.png" height="400"></p>


## **Creating our first website**

### **Pre-reqs**


- Before configuring IIS, we need to create a directory to host our website files. Open File Explorer, navigate to `This PC`, `Windows (C:)`, then create a new folder named `Websites`. Inside of that folder, create a new folder named `MyWebsite`. All your website files will live inside of this directory.


<p align="center"><img src="assets/images/windowdir.png" height="400"><img src="assets/images/windowsnewfolder.png" height="400"></p>


### **Making the site**

1. After installation of IIS, creating and hosting your own website is fairly simple.
2. Hit the windows key and type in `IIS` and select `Internet Information Services (IIS) Manager`, which should bring up a control panel for all IIS services.


<p align="center"><img src="assets/images/IISManager.png" height="400"></p>


3. ***Disable the `Default Web Site` by right clicking `Default Web Site`, selecting `Manage Website`, then `Stop`***


<p align="center"><img src="assets/images/disabledefault.png" height="400"></p>


4. Right click on `Sites`, and select `Add Website`. This should bring up a control panel named `Add Website`, shown below.


<p align="center"><img src="assets/images/IISSites.png" width="400"></p>

<p align="center"><img src="assets/images/IISAddSite.png" height="450"><img src="assets/images/IISAddSiteFilled.png" height="450"></p>


6. Download the sample html webpage [here](https://raw.githubusercontent.com/SIGSAC/SIGSAC/master/5.%20Your%20Very%20Own%20Website/Exercise/assets/files/index.html?token=ANDKV24Y6KXOBCODH3ROX6K7I6ZIY), and place it into the new directory, `C:\Websites\MyWebsite`
7. Navigate to `http://localhost` once more and you should see your new website. Congrats!

## **Troubleshooting**



## **Uninstalling IIS**

- Hit the windows key and start typing `Turn Windows` and select `Turn Windows features on or off`.
- Scroll to find `Internet Information Services`.
- Check the box to empty
- Press OK.
- Allow computer to reboot as necessary.


<!--So what does IIS do? It simply shows people who show up, the files that live in your websites directory. Think of it as someone showing up to your house, and then looking at your doormat. -->

<!--Also, congrats if you found this lmao -->
