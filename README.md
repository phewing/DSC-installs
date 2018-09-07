# DSC-installs


## Summary

This repository includes program installation files and Grasshopper plugins for running DSC analysis workflow at Auburn University.

## System Installations

The following programs will have to be installed to the Windows PC (or virtual machine):

+ [DAYSIM v4.0](https://daysim.ning.com/page/download)
+ [EnergyPlus v8.9.0](https://energyplus.net/downloads)
+ [Radiance v5.1.0](https://github.com/NREL/Radiance/releases)
  + __NOTE 1:__ Radiance should be installed directly to the 'main' C: drive if possible (e.g., `C:\Radiance\bin`, `C:\Radiance\lib`, etc.), instead of a Progam files sub-folder, in order for Honeybee/Ladybug plugins to be guaranteed to work; alternate installation paths have not yet been tested for this workflow.
  + __NOTE 2:__ Since Radiance is a 'UNIX-style' command-line application, ensure that (1) there is an enviroment variable named `RAYPATH` which points to `C:\Radiance`, and (2) that `C:\Radiance\bin` and `C:\Radiance\lib` are included in the system's `%PATH%` variable.
+ [Open Studio v2.5.0](https://daysim.ning.com/page/download)

## Plugin Installations

These are Grasshopper plugins that can be installed by adding the `.gha` or `.xml` files to the user's `%APPDATA%/Grasshopper/Components` directory, or `.ghuser` files to the user's `%APPDATA%/Grasshopper/UserObjects` directory:

+ Honeybee Ladubyg legacy 0063
+ Honeybee and Ladybug plus 0004
+ Lunchbox
+ Tree8
+ Human UI
+ TT Toolbox 1-9

Since it appears that Auburn architecture VMs cannot store these files in user-account-specific folders, these can be copied over either (1) manually by the students, or (2) stored in a system folder that remains persistent between logins, and copied over via startup shell script upon login.

A short batch script that can be added to the Windows startup schedule to make the copy-over for Grasshopper plugins to %APPDATA%/Grasshopper subdirectorys will be uploaded to this repository shortly!
