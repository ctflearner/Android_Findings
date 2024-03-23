# OpenBot
## Project-Details:
- Project-Name : OpenBot
- Package-Name : org.openbot
- Version-Affected : v0.7.1
- Github-Repo : https://github.com/isl-org/OpenBot
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Title : Accepting all SSL Certificates


## Description:
The APK is set to accept all SSL certificates. This allow connection to the websites which are signed by untrust Certificate Authorities, 
that can lead to compromise of data.

## Mitigation
An app that does not want to trust all CAs trusted by system can instead specify its own reduced set of CAs to trust .
This protects the app from fraudlent certificates issued by any of the other CAs.

### CWE-295: Improper Certificate Validation 
Associated Files

1. **sources/cz/msebera/android/httpclient/conn/ssl/SSLConnectionSocketFactory.java**
2. **sources/cz/msebera/android/httpclient/conn/ssl/SSLSocketFactory.java**
3. **sources/com/loopj/android/http/MySSLSocketFactory.java**

### Proof_OF_Concept

![OpenBOT_SSL_Certificates_SSL_Connection_Socket_Factory-01](https://github.com/ctflearner/Android_Findings/assets/98345027/979b263c-725c-428f-b036-f357b086a7e6)

![OpenBOT_SSL_Certificates_SSL_SOCKET_Factory_02](https://github.com/ctflearner/Android_Findings/assets/98345027/07b4e7be-c7fc-4c48-8d8a-71eb2af8f781)
