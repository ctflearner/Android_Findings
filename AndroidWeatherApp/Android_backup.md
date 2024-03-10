## AndroidWeatherApp
### Github_Repo_of_the_Project : https://github.com/jurecapuder/AndroidWeatherApp
## Project-Details:
- Project-Name : AndroidWeatherApp
- Package-Name : com.example.weatherapp
- Version-Affected : v1.0.0 
- Language-Used : Java

## Vulnerability : Android Backup Vulnerability
### Description:
An Android backup vulnerability is found in the androidmanifest.xml file of AndroidWeatherApp apk file. The property android:allowBackup='true' exists on the application tag in the androidmanifest.xml file, which means that the Android application users can back up the app's internal data, which resides under /data/data/.

### Impact:
An attacker with physical access to the device could perform a data backup, gathering login credentials and other sensitive information

### Remediation:
To avoid Android backup vulnerability, set android:allowBackup=false within the androidmanifest.xml file.

### Severity: Medium

## Proof_Of_Concept
![AndroidWeatherApp_Manifest_POC-1](https://github.com/ctflearner/Android_Findings/assets/98345027/6667af77-94f9-4d07-ac91-da2feebf1825)
