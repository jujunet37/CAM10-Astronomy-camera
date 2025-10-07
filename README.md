# CAM10-Astronomy-camera

## This repository contains all files needed to build two differents astronomy monochrome Cam10 cameras with a resolution of 1280x1024. Original wiring diagram was made by grim from Astroclub.kiev.ua.
CAUTION : For Autoguiding use the ASCOM version. The COM version is only for standalone use with the viewer.

## UPDATE 07/10/2025 :

The driver has been updated to work with PHD2. The workaround with PHD1 explained in the video is not necessary anymore. 
Driver version 0.5 didn't work because camera settings woulnd't open, and camera settings button was grayed out.
I made modifications on this driver to open the camera settings on loading. So now you can tune the image directly in PHD2.
Enjoy !

Note : I noticed my anti virus show a false positive on my mini PC (Windows Defender). It's normal with ASCOM unsigned drivers.
You can put it in white list to install if you have the message.

# Cam10 COM version :

Description : This camera can be use for planetary Imaging, there is no ASCOM driver. The viewer communicate with a virtual serial COM port. Using the pcb provided by grim I made a 3D printed enclosure for this camera. All parts needed are in the folder.

## Folders :

- Cam 10 COM Viewer : The viewer, it's a standalone viewer developped by grim to capture images on jpg, bmp, fit and ser formats. ROI capability and exposure / ISO settings. Gain/offset/delta/timer parameters.
- Components list : I provided the list of elements, with screen captures to avoid dead links, so you can easyly retrieve the parts needed.
- Firmware : The firmware and the utility to flash it on the camera (ST-LINK)
- PCB Gerber File : The Gerber file to make the PCB
- STL files Cam10 COM version : The stl files to print the enclosure


# Cam10 ASCOM version :

Description : This camera can be used for both planetary imaging and autoguiding. A viewer can be used for standalone acquisition. An ASCOM driver is provided, works with ASCOM 6.2. I used the original wiring from grim and corrected a missing track. I made a new corrected PCB with mounting holes to install a heatsink. I also made an 3D printed enclosure.

## Folders :

- ASCOM driver : This is the ascom driver to make it communicate with all astronomy softwares (Sharpcap, OpenNebulosity, PHD2). Version 0.5
- Components list : I provided the list of elements, with screen captures to avoid dead links, so you can easyly retrieve the parts needed.
- Firmware + MPROG : This is the firmware and the programming utility for flashing the FT2232 chip
- FT2232 Driver : Drivers for Windows for the FT2232. I provided 2 drivers, you can check for updates on FTDI website, type FT2232HL and install lastest drivers. WARNING : Since several years FTDI brick non genuine chips. If you purchased your chip on an official reseller, you can update to last driver. If your chip comes from Aliexpress or EBay, be careful about that, if you have any doubt, install the 2.08 provided driver.
- Old ASCOM Platform : This is the old ASCOM platform that works with this camera, not tested with newer versions.
- PCB Gerber file : The Gerber file to make the PCB
- Schema : Original diagram by grim
- STL Files CAM 10 ASCOM : The stl files to print the enclosure
- Viewer Source and Exec : Viewer souce files and main executable.

## Softwares folder : 

- This is PHD first version (very hard to found on the web). Use for the workaround to make the ascom parameter works in PHD2. Look at YouTube video link below.

Links :

Youtube tutorials :

French : https://www.youtube.com/watch?v=oHPourlEOjQ
English : https://www.youtube.com/watch?v=FNpK9c-Fqkc

Astroccd : http://astroccd.org/
Ukrainian Astropolis topic : https://www.astroclub.kiev.ua/forum/index.php?PHPSESSID=su8vh9h1n0l7lrnate4rmb50v5&topic=28929.0