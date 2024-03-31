## Project-Details:
- Project-Name : QKSMS
- Package-Name : com.moez.QKSMS
- Version-Affected : v3.9.4
- Language-Used : Java,kotlin

## Title: Application Data can be Backed up
### Description:
An Android backup vulnerability is found in the androidmanifest.xml file of QKSMS v3.9.4 apk file. The property android:allowBackup='true' exists on the application tag in the androidmanifest.xml file, 
which means that the Android application users can back up the app's internal data, which resides under /data/data/.

### Impact:
An attacker with physical access to the device could perform a data backup, gathering login credentials and other sensitive information

### Remediation:
To avoid Android backup vulnerability, set android:allowBackup=false within the androidmanifest.xml file.

## Proof_of_Concept
![QKSMS-backup-01](https://github.com/ctflearner/Android_Findings/assets/98345027/3eaf9981-81a8-4733-9f11-328ebe36f44e)
