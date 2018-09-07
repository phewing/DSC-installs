# DSC-installs


## Summary

This repository includes program installation files and Grasshopper plugins for running DSC analysis workflow at Auburn University.

## System Installations

The following programs will have to be installed to the Windows PC (or virtual machine):

+ [DAYSIM v4.0](https://daysim.ning.com/page/download)
+ [EnergyPlus v8.9.0](https://energyplus.net/downloads)
+ [Radiance v5.1.0](https://github.com/NREL/Radiance/releases)
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

A shell script to make the copy-over for Grasshopper plugins to %APPDATA%/Grasshopper subdirectorys will be uploaded to this repository shortly!
