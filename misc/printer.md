# How to add the Printer
1. ***MAKE SURE YOU ARE CONNECTED TO EECSNET TO PRINT ANYTHING*** 
1. [Download the Driver](https://www.support.xerox.com/support/workcentre-6515/file-download/enus.html?operatingSystem=linux&fileLanguage=en&contentId=144039&from=downloads&viewArchived=false)
2. Restart CUPS in your terminal
    ```
    sudo systemctl restart cups
    ```
3. Go to [localhost:631](localhost:631)
   1. Adding Printers and Classes ![](pictures/Printer1.png)
   2. Add Printer ![](pictures/Printer2.png)
   3. Choose LPD/LPR Host or Printer ![](pictures/Printer3.png)
   4. Type ```lpd://10.13.255.50/queue``` into **Connection** ![](pictures/Printer3.png)
   5. Name the printer ```Thayer115``` ![](pictures/Printer3.png)
   6. Browse for a PPD File from /opt/Xerox/prtsys/ppd/XRWC6515.ppd ![](pictures/Printer3.png)
   7. Set Duplex to ```long edge```![](pictures/Printer3.png)
   8. 