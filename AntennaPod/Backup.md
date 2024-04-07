## Project-Details:

- Project-Name : AntennaPod
- Package-Name : de.danoeh.antennapod
- Version-Affected : v3.3.2

## Title: Application Data can be Backed up

### Description:

An Android backup vulnerability is found in the androidmanifest.xml file of AntennaPod v3.3.2 apk file. The property android:allowBackup='true' exists on the application tag in the androidmanifest.xml file,
which means that the Android application users can back up the app's internal data, which resides under /data/data/.

### Impact:

An attacker with physical access to the device could perform a data backup, gathering login credentials and other sensitive information

### Remediation:

To avoid Android backup vulnerability, set android:allowBackup=false within the androidmanifest.xml file.

## Proof_of_Concept
![Antenna_Bckup](https://github.com/ctflearner/Android_Findings/assets/98345027/f956df47-8cf8-4689-8973-0dca8cda1e47)
