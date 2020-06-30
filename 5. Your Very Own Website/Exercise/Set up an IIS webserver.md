# Setting up a webpage in Windows Internet Information Services (IIS)

*Written and tested by [43y3s](https://github.com/incub4t0r)*

## **Table of Contents**

1. [Internet Information Services (IIS)](#IIS)
    1. [Background](#Background)
    1. [Installing IIS](#Installing-IIS)
    1. [Checking installation](#Checking-installation)
2. [Creating your first website](#Creating-our-first-website)
    1. [Pre-reqs](#Pre-reqs)
    2. [Making the site](#Making-the-site)
3. [Troubleshooting](#Troubleshooting)
4. [Uninstalling IIS](#Uninstalling-IIS)

## **IIS**
### Background
Websites are comprised of code (html, css, python etc). In order to convert the code into a visible site, you need to use a service/software that can process the code. Of the three most popular webserver softwares (Apache, Nginx, IIS), IIS is the one that can *only* run on Windows operating systems.

| IIS | Apache | Nginx |
| :-: | :-: | :-: |
| <img src="https://www.saotn.org/wp-content/uploads/2014/07/IIS_logo.png" width="500"> | <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/d/db/Apache_HTTP_server_logo_%282016%29.svg/1200px-Apache_HTTP_server_logo_%282016%29.svg.png" width="500"> | <img src="https://www.nginx.com/wp-content/uploads/2018/08/NGINX-logo-rgb-large.png" alt="drawing" width="500"> |

### Installing IIS

1.  Hit the windows key and start typing `Turn Windows` and select `Turn Windows features on or off`.
2.  Scroll to find `Internet Information Services`.
3.  Make sure the `Internet Information Services` box is checked. `FTP Server` should not be checked, but `Web Management Tools` and `World Wide Web Services` should be.

| Step 3 |
| :-: |
| <img src="assets/images/windowsfeatures.png" width="400"> |

4.  Press OK, and reboot computer.

### Checking installation

Open a browser tab, and navigate to `http://localhost` in the search bar, and you should be met with a blue webpage shown below.

| Check to see IIS is running |
| :-: |
| <img src="assets/images/iisstart.png" width="400"> |



## **Creating your first website**
Now that you have your webserver, you can upload the code for your website! But first...
### Pre-reqs
Before configuring the IIS software, you need to create a directory (folder) to host your website code.
1. Open File Explorer
2. Navigate to `This PC`, then `Windows (C:)`
3. Create a new folder named `Websites`. Inside of that folder, create a new folder named `SIGSAC_Site_1`

All your website files will live inside of this directory.

| Step 1 | Step 2 |
| :-: | :-: |
| <img src="assets/images/windowdir.png" width="500"> | <img src="assets/images/windowsnewfolder.png" width="500"> |


### **Making the site**

1. After installation of IIS, creating and hosting your own website is fairly simple.
2. Hit the windows key and type in `IIS` and select `Internet Information Services (IIS) Manager`, which should bring up a control panel for all IIS services.


<p align="center"><img src="assets/images/IISManager.png" width="400"></p>


3. ***Disable the `Default Web Site` by right clicking `Default Web Site`, selecting `Manage Website`, then `Stop`***


<p align="center"><img src="assets/images/disabledefault.png" width="400"></p>


4. Right click on `Sites`, and select `Add Website`. This should bring up a control panel named `Add Website`, shown below.


<p align="center"><img src="assets/images/IISSites.png" width="400"></p>

<p align="center"><img src="assets/images/IISAddSite.png" width="450"><img src="assets/images/IISAddSiteFilled.png" width="450"></p>


6. Download the sample html webpage [here](https://github.com/PillowFood/SIGSAC/raw/master/5.%20Your%20Very%20Own%20Website/assets/files/index.html), and place it into the new directory, `C:\Websites\MyWebsite`
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
