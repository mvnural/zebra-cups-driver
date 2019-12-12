# zebra-cups-driver
The default Zebra driver distributed with the CUPS installations may cause issues with some of the smaller size labels commonly used in research/clinical settings. This modified driver fixes that issue.

## GUI Installation (Mac)
1. Make sure the printer is turned on and connected to the computer.
1. Download Zebra Printer Driver file (zebra_zpl_II.ppd) from the following link:
https://github.com/mvnural/zebra-cups-driver/raw/master/zebra_zpl_II.ppd
1. Go to System Preferences -> Printers & Scanners and click the plus sign to add a new printer.
![GUI-1](/images/gui_1.png)

1. Highlight the Zebra Printer and click "Other..." from the "Choose a Driver" dropdown.
![GUI-2](/images/gui_2.png)

1. Locate & highlight the driver file (zebra_zpl_II.ppd) you have just downloaded and click open to
select.
![GUI-3](/images/gui_3.png)

1. Click "Add" to complete installation of the printer.
![GUI-4](/images/gui_4.png)

## Installation via CUPS Web Interface (Mac & Linux)
1. Make sure the printer is turned on and connected to the computer.
1. Download Zebra Printer Driver file (zebra_zpl_II.ppd) from the following link:
https://github.com/mvnural/zebra-cups-driver/raw/master/zebra_zpl_II.ppd
1. Point your browser to http://localhost:631 to open CUPS Web Interface
![CUPS-1](/images/cups_1.png)

1. Click Administration -> Add Printer. If you get an error saying the webinterface is disabled, simply copy and paste the `cupsctl WebInterface=yes` command in your terminal to enable it. 
![CUPS-2](/images/cups_2.png)

1. Find the Zebra printer to add and in the final screen, click "Choose File" in the "Provide a PPD file" section and point to the the driver file (zebra_zpl_II.ppd) you have just downloaded instead of choosing one of the existing drivers.
![CUPS-3](/images/cups_3.png)

1. Click "Add Printer" to complete installation of the printer.
