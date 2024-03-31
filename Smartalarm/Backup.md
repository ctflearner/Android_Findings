## Project-Details:
- Project-Name : smartalarm
- Package-Name : com.fridgecow.smartalarm
- Version-Affected : v1.8.1
- Language-Used : Java

## Title: Application Data can be Backed up
### Description:
An Android backup vulnerability is found in the androidmanifest.xml file of smartalarm v1.8.1 apk file. The property android:allowBackup='true' exists on the application tag in the androidmanifest.xml file,
which means that the Android application users can back up the app's internal data, which resides under /data/data/.
### Impact:
An attacker with physical access to the device could perform a data backup, gathering login credentials and other sensitive information

### Remediation:
To avoid Android backup vulnerability, set android:allowBackup=false within the androidmanifest.xml file.

### Proof_Of_Concept

![smartalarm_allow_backup_01](https://github.com/ctflearner/Android_Findings/assets/98345027/e2a1552f-ec50-40ef-9682-48b34fbf9d9a)
