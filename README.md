# centos7-usb-kickstart
Files needed to boot a system from USB and autoconfig via kickstart

## How to use this:

1. Download and install Rufus on a Windows system (instructions using dd are in-process)
 * https://downloads.tomsguide.com/Rufus,0301-53760.html

2. Download Centos 7 minimal iso 
 * http://isoredirect.centos.org/centos/7/isos/x86_64/CentOS-7-x86_64-Minimal-1810.iso

3. Use Rufus to build bootable USB (using a USB thumb drive of at least 2GB). Use Isohybrid mode.

4. Open the drive and transfer filed into the isolinux directory
 * isolinux.cfg
 * ks.cfg
 
 (customize these files as you wish but be aware that windows can mess with CR/LF)

## How to customize this

Boot menu is found within isolinux.cfg. Use this to cutomize boot menu or special kernel options

Actual install of Centos7 is found within ks.cfg (kickstart file). Customize what gets installed.

