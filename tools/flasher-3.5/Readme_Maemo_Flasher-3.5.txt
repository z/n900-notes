Maemo Flasher-3.5 Tool

  Copyright (C) 2009 Nokia Corporation. All rights reserved.

  Nokia and maemo are trademarks or registered trademarks of Nokia Corporation. 
  Other product and company names mentioned herein may be trademarks or trade 
  names of their respective owners. 


* DISCLAIMER

  This software is work-in-progress and use of this software requires special 
  skills and knowledge. The software and the instructions provided herein or 
  with the software may not be complete. Improper use or installation of this 
  software may harm the device you are installing it into, or the device you are 
  using it with. By accepting the License Agreement deliverd together with this 
  software you also agree to use this software at your own risk and accept that 
  Nokia assumes no liability and does not provide any warranties, support or 
  services related to the software.

* MAEMO FLASHER-3.5 DETAILS

  - Version: 2.5.2 - Final
  - Date: October 23, 2009
  - Hardware supported: Nokia N800, N810 and N810 WiMAX with Diablo 4.1.x and
                        N900 with Fremantle 5.x

* SUPPORTED OPERATING SYSTEMS

  - Linuxes (Debian installation package available for Debian based Linuxes and tar ball for others)
  - Windows XP with SP3, Vista with SP2 and Windows 7
  - Mac OS X 10.5 Leopard and 10.6 Snow Leopard
  
  Notice: Linux and Windows versions of Flasher-3.5 Tool support x86/32-bit host PC architectures.  
          Mac OS X versions support x86/32-bit and PPC/32-bit architectures.

* FILES INCLUDED

  - flasher-3.5                  - flasher binary file (flasher-3.5.exe for Windows)
  - libusb                       - USB library (only for Windows and Mac OS X installations)
  - COPYING_LGPL.txt             - license text for libusb (only for Windows and Mac OS X installations)
  - License_Agreement.txt        - license and disclaimer text for flasher binary
  - Help.txt                     - short command line help 
  - Readme_Maemo_Flasher-3.5.txt - this file

* DOWNLOADS AND DOCUMENTATION
    
  - Flasher-3.5 download: http://tablets-dev.nokia.com/maemo-dev-env-downloads.php
  - Flasher-3.5 documentation: see command line help file
          
  - Sources for libusb library (LGPL v2) installed as part of Flasher-3.5 for 
    Windows and Mac OS X:
    * Libusb (Mac): http://pc-connectivity.garage.maemo.org/upstream/libusb-0.1.12.tar.gz
    * Libusb-win32 (Win): http://pc-connectivity.garage.maemo.org/upstream/libusb-win32-src-0.1.12.1.tar.gz
    
  - Original libusb sources are available from SourceForge.net:
    * Libusb (Mac): http://ufpr.dl.sourceforge.net/sourceforge/libusb
    * Libusb-win32 (Win): http://ufpr.dl.sourceforge.net/sourceforge/libusb-win32

* INSTALLATION

  The Flasher-3.5 tool should be installed from the installation package 
  provided for Debian based Linuxes, Windows and Mac OS X. For other than 
  Debian based Linux distributions also compressed tar file is provided. 
    
  Installation of Maemo Flasher-3.5 requires administration rights in all 
  supported operating systems.

* SHORT DESCRIPTION

  The Maemo Flasher-3.5 Tool is a command line utility that supports N900 device 
  with Fremantle 5.x platform releases and N800, N810 and N810 WiMAX devices 
  with Maemo Diablo 4.1.x platform releases.
    
  Notice that older Maemo devices (like Nokia 770) and older Maemo platform 
  releases may require a specific Flasher Tool.

  Flasher-3.5 Tool is run from a Linux, Windows or Mac host computer as command 
  line tool, and it will send data and commands to the connected Maemo device 
  over USB. 
    
  Flasher-3.5 Tool can be used to:
    1. flash Maemo device with Diablo or Fremantle FIASCO image
    2. flash Maemo device (N900 only) internal memory card with eMMC image
    3. unpack FIASCO image into separate parts like kernel and rootfs images
    4. flash unpacked kernel or rootfs images to the Maemo device separately
    5. change Mameo device into R&D mode and back to normal mode
    6. set and clear R&D flags for Maemo device when in R&D mode
    7. boot Maemo device with additional kernel startup parameters 
    8. and for many other purposes
    
  All command line parameters supported by Flasher-3.5 Tool together with some 
  basic usage examples are documented in Help.txt file available as part of tool 
  installation package. Flasher-3.5 Tool binary gives command line help if it is 
  run without any parameter or with "--set-rd-flags" or "--clear-rd-flags" 
  parameters.
    
  Before flashing Maemo device with FIASCO image it is recommended to set Maemo 
  device first into flashing mode. 
    
  For Nokia N800 and N810 with Diablo image flashing mode can be enabled by 
	  1. Turn off Maemo device (and do not use charger)
	  2. Attach USB cable on your Maemo device and computer
	  3. Turn on Maemo device while holding down the Home (N800) or 
	     Swap (N810) hardware button  
	
  For Nokia N900 with Fremantle image flashing mode can be enabled by
   1. Turn off Maemo device 
   2. Press and hold down key 'u' 
   3. Connect USB cable between Maemo device and host PC while holding down key 'u'
   4. When USB cable gets connected it powers Maemo device and set's it to flashing mode
   5. When USB icon appears on right upper corner Maemo device is in flashing mode 
   6. You can release key 'u'
 
	You will see USB image in the upper right hand corner of the screen if you did 
	this correctly.
	    
  Maemo device will wait for Flasher-3.5 input indefinitely when it is in 
  flashing mode. If flashing is tried without setting Maemo device first into 
  flashing mode image flashing may fail because Maemo device may not be able to 
  change to the flashing mode automatically.
   
  NOTICE: Make sure that device battery is fully charged before doing any 
          sort of flashing operation because flashing will fail if battery
          runs out of power during image flashing operation and device 
          may not be able to charge empty battery after failure in flashing. 

* TIPS & TROUBLESHOOTING
    
  If you get a "Permission denied" error then make sure you have execution 
  rights to the flasher-3.5 binary executable. You may also need to have 
  administrator permissions or run command with sudo in Linux.
    
  It may help to connect USB cable directly to the computer USB ports, avoiding 
  the use of a hub. The USB ports in the back of a computer may also work better 
  than using those in the front.

----
Feedback from Flasher-3.5 Tool can be sent to integration@maemo.org