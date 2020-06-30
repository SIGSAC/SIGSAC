# Setting up a webpage in Windows Internet Information Services (IIS)

*Written and tested by [43y3s](https://github.com/incub4t0r)*

## **Table of Contents**

1. [Internet Information Services (IIS)](#IIS)
    1. [Background](#Background)
    1. [Installing IIS](#Installing-IIS)
    1. [Checking installation](#Checking-installation)
2. [Creating your first website](#Creating-our-first-website)
    1. [Pre-reqs](#Pre-reqs)
    2. [Configure your website](Configure-your-website)
      1. [Disable the default code](#Disable-the-default-code)
      2. [Add the code](#Add-the-code)
      3. [Host the site](#Host-the-site)
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

| Step 2 |
| :-: |
| <img src="assets/images/windowsnewfolder.png" width="500"> |


### Configure your website
All that is left is for you to replace the default html code with your own code. Then IIS will help you host your very own website!

#### Disable the default code
1. Hit the windows key and type in `IIS` and select `Internet Information Services (IIS) Manager`. This will bring up a control panel for all IIS services.
2. Disable the `Default Web Site` by right clicking `Default Web Site`, selecting `Manage Website`, then `Stop`

| Step 1 | Step 2 |
| :-: | :-: |
| <img src="assets/images/IISManager.png" width="500"></img> | <img src="assets/images/disabledefault.png" width="500"></img> |

#### Add your own code
3. Copy and paste the following code into a text editor, and then save it as "index.html" in `C:\Websites\MyWebsite`. You can also find the code [here](https://github.com/SIGSAC/SIGSAC/blob/master/5.%20Your%20Very%20Own%20Website/Exercise/assets/files/index.html)

| Step 3 |
| :-: |
|  <img src="assets/images/websitecode.png" width="500"> |

#### Host the site
4. Right click on `Sites`, and select `Add Website`. This should bring up a control panel named `Add Website`.

| Step 4 | Step 5 |
| :-: | :-: |
| <img src="assets/images/IISSites.png" width="500"> | <img src="assets/images/IISAddSiteFilled.png" width="500"></img> |

6. Navigate to `http://localhost` once more and you should see your new website. Congrats!
| Step 6 |
| :-: |
| <img src="assets/images/localhostwebsitepng.png" width="500"> |


## **Additional Info**
- You can save your html files anywhere on the computer. It doesn't need to be in `C:\Websites\MyWebsite`
- Your website is hosted locally (AKA localhost). That means only your computer can see it, no other device. 

## **Uninstalling IIS**
If you ever need to uninstall IIS, these are the steps

1. Hit the windows key and start typing `Turn Windows` and select `Turn Windows features on or off`.
2. Scroll to find `Internet Information Services`.
3. Check the box to empty
4. Press OK.
5. Allow computer to reboot as necessary.


<!--So what does IIS do? It simply shows people who show up, the files that live in your websites directory. Think of it as someone showing up to your house, and then looking at your doormat. -->

<!--Also, congrats if you found this lmao -->
