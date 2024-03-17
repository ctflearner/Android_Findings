# OpenBot
## Project-Details:
- Project-Name : OpenBot
- Package-Name : org.openbot
- Version-Affected : v0.7.1
- Github-Repo : https://github.com/isl-org/OpenBot
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Vulnerability :  Weak Hashing Algorithms 
## Description:
It has been found that this application OpenBot v0.7.1 , uses the MD5 MessageDigest algorithm and SHA-1 which is weak. This Weak Algorithm is used in SIX Location of the File .

The File Path of the Above issue is given below:

1. **com\github\faucamp\simplertmp\Util.java** 
2. **com\google\android\gms\measurement\internal\zzkk.java**
3. **com\koushikdutta\async\util\FileCache.java**
4. **com\pedro\rtsp\utils\AuthUtil.java**
5. **cz\msebera\android\httpclient\impl\auth\NTLMEngineImpl.java** 
6. **com\google\firebase\installations\local\IidStore.java**

### **Remediation:**

Use stronger hash algorithm's .

### **Severity: Medium**

## Proof_Of_Concept
![Openbot_Weak_Algo_util_1](https://github.com/ctflearner/Android_Findings/assets/98345027/a46f2eb9-1e99-456a-90cc-5bfb1724dc8a)

![Openbot_Weak_Algo_util_1 1](https://github.com/ctflearner/Android_Findings/assets/98345027/f0e041db-e677-403b-9846-6c905db612c4)

![Openbot_Weak_Algo_zzkk_2](https://github.com/ctflearner/Android_Findings/assets/98345027/f866c928-b1f6-477d-bf76-64af94cc5a6b)

![Openbot_Weak_Algo_FileCache_3](https://github.com/ctflearner/Android_Findings/assets/98345027/32aa2ae4-70e5-4d0e-9d68-89ac17e855c8)

![Openbot_Weak_Algo_AuthUtil_4](https://github.com/ctflearner/Android_Findings/assets/98345027/b441ae2a-970c-47e0-830b-dee740ab2e10)

![Openbot_Weak_Algo_NTLMEngineImpl_5](https://github.com/ctflearner/Android_Findings/assets/98345027/82b0c25d-5cb0-4837-9645-cc0362ec113b)

![Openbot_Weak_Algo_NTLMEngineImpl_5 1](https://github.com/ctflearner/Android_Findings/assets/98345027/1b124ea9-b00c-4875-afc7-f990a5b1bb66)

![Openbot_Weak_Algo_lidStore_6](https://github.com/ctflearner/Android_Findings/assets/98345027/47e628b7-b013-45ef-a598-6cc1a07a7e27)







