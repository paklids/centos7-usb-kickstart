# centos7-usb-kickstart
Files needed to boot a system from USB and autoconfig via kickstart

## How to use this:

1. Download and install Rufus on a Windows system (instructions using dd are in-process)
 * https://downloads.tomsguide.com/Rufus,0301-53760.html

2. Download Centos 7 minimal iso 
 * http://isoredirect.centos.org/centos/7/isos/x86_64/CentOS-7-x86_64-Minimal-1810.iso

3. Use Rufus to build bootable USB (using a USB thumb drive of at least 2GB). Use Isohybrid mode.

4. Open the drive and transfer filed into the isolinux directory
 * `isolinux.cfg`
 * `ks.cfg`
 
 (customize these files as you wish but be aware that windows can mess with CR/LF)

 5. Boot the target system from USB and follow the prompts. System will need network access to pull 
    additional packages that are not included in the Minimal ISO.

## What does this build?

This builds a very basic Centos7 workstation with a browser and a few useful tools

## How to customize this

Boot menu is found within `isolinux.cfg` . Use this to cutomize boot menu or special kernel options

Actual install of Centos7 is found within `ks.cf`g (kickstart file). Customize what gets installed.

