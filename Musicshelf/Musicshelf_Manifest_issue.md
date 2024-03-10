# Musicshelf_Manifest_Misconfiguration

Github_Repo_of_the_Project : https://github.com/KirillMakarov/Musicshelf 
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
## Project-Details:
- Project-Name : Musicshelf
- Package-Name : com.kamakarov.musicshelf
- Version-Affected : 1.1
- Language-Used : Java
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
## Vulnerability : Android Backup Vulnerability 
## Description: 
An Android backup vulnerability is found  in the androidmanifest.xml file of Musicshelf apk file. The property android:allowBackup='true' exists on the application tag in the androidmanifest.xml file, which means that the Android application users can back up the app's internal data, which resides under /data/data/<app-package>.
## Impact: 
An attacker with physical access to the device could perform a data backup, gathering login credentials and other sensitive information
## Remediation: 
To avoid Android backup vulnerability, set android:allowBackup=false within the androidmanifest.xml file.
## Severity: Medium
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
## Proof_Of_Concept
![Musicshelf-Android-Manifest-POC-1](https://github.com/ctflearner/Android_Findings/assets/98345027/565a64cf-8a96-46d5-a465-dc95d35d35ff)
