### Project Details
- Vulnerablle_Version: v1.0
- Package-Name: com.innovate.replify

## Title: Application Data can be Backed up

### Description:

An Android backup vulnerability is found in the androidmanifest.xml file of Replify-Messenger v1.0 apk file. The property android:allowBackup='true' exists on the application tag in the androidmanifest.xml file,
which means that the Android application users can back up the app's internal data, which resides under /data/data/.

### Impact:

An attacker with physical access to the device could perform a data backup, gathering login credentials and other sensitive information

### Remediation:

To avoid Android backup vulnerability, set android:allowBackup=false within the androidmanifest.xml file.

### Proof_Of_Concept
![Replify-Messenger-Bacup01](https://github.com/ctflearner/Android_Findings/assets/98345027/831443fb-b2f9-409d-a640-8ed1b9a8490c)
