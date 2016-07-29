# Flashing the odroid

We provide an image file of the odroid which you can flash onto your odroid using the steps described below. By downloading and flashing this image file onto the odroid's eMMC chip, you will have an exact copy of the entire operating system, including installed software, packages, and tools (e.g. ROS, openCV, Julia, etc)  necessary to run experiments. The image file is available [here](http://dator.forge9.com/static/odroid_3_18.img). The image file is large (~14GB), so it is recommended to download it overnight with a stable connection. To verify a successful download, check the MD5 hash value (for Windows refer to [here](https://support.microsoft.com/en-us/kb/889768), for Mac/Linux use the md5 / md5sum command). You should the exact MD5 value below; if not, something probably got corrupted during the download, try re-downloading

 014a8d3030e348660493b17575b43759

Before flashing the eMMC, you will need to a labtop, a microSD-to-eMMC adaptor and a microSD card reader (if your laptop doesn't have an SD port). The main steps for flashing are as follows 
1. Remove eMMC from odroid
<img src="http://dn.odroid.com/homebackup/201412042047141455.jpg"/>
2. Connect eMMC to microSD-to-eMMC adapter 
<img src="http://static.generation-robots.com/5914-thickbox_default/8-gb-odroid-xu3xu4-emmc-module.jpg" width="200" height="200" />
3. Attach eMMC adapter (with eMMC) to laptop (using the microSD-to-USB adapter if necessary)
4. Flash the image
    * [Win32DiskImager](https://sourceforge.net/projects/win32diskimager/) (Windows)
    * [Disk Utility](http://osxdaily.com/2012/01/04/format-an-external-hard-drive-or-usb-flash-drive-for-mac-os-x/) (Mac)
    * dd command (Mac/Linux, instructions [here](https://help.ubuntu.com/community/DriveImaging) )
5. Re-attached eMMC the odroid

Before turning on the odroid, attach real-time clock battery to the corresponding port on the odroid (at mid-top edge, see image below). 
Next, use a HDMI-to-DVI cable to connect your odroid to a monitor. 
Use the outlet adapter to power the odroid via the 5V4A DC Input port (mid-left). 
If everything goes smoothly, you should a desktop background similar to the one below

### Odroid Diagram
![alt tag](https://www.crazypi.com/image/cache/data/Odroid/XU4/xu4_3-autoxauto.jpg)

### Default Desktop background
<img src="http://www.cnx-software.com/wp-content/uploads/2014/12/ODROID-XU3_Lite_Ubuntu_Desktop.png"/>