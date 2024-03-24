# Project-Details 
- Github-Repo : https://github.com/xbmc/xbmc 
- Version: v20.5-Nexus 

## Title 
- This Application v20.5-Nexus Data can be Backed up
[android:allowBackup] flag is missing.

## Description
- The flag [android:allowBackup] should be set to false.
By default it is set to true and allows anyone to backup your application data via adb. It allows users who have enabled USB debugging to copy application data off of the device.

## Proof Of Concept
![kodi-manifest](https://github.com/ctflearner/Android_Findings/assets/98345027/c6dc7b5c-8eb4-4cb6-82dc-748c5a79189d)
