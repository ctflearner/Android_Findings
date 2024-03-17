
# OpenBot
## Project-Details:
- Project-Name : OpenBot
- Package-Name : org.openbot
- Version-Affected : v0.7.1
- Github-Repo : https://github.com/isl-org/OpenBot
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

## Description:

It has been found that this application OpenBot v0.7.1 is using a function called Random() , which is used to generate the random numbers in java, which has been taken from java library called java.util.Random. By using this java.util.Random class makes the random number generation cryptographically weak.

File Location :

1. **androidx\activity\result\ActivityResultRegistry.java**
2. **com\annimon\stream\RandomCompat.java**
3. **com\github\anastr\speedviewlib\Gauge.java**
4. **com\github\faucamp\simplertmp\io\RtmpConnection.java**
5. **com\github\faucamp\simplertmp\packets\Handshake.java**
6. **com\koushikdutta\async\dns\Dns.java**
7.  **com\koushikdutta\async\util\FileCache.java**
8. **com\loopj\android\http\SimpleMultipartEntity.java**
9. **com\pedro\rtsp\rtsp\RtspSender$start$$inlined$let$lambda$1.java**
10.  **cz\msebera\android\httpclient\entity\mime\MultipartEntityBuilder.java**
11.  **kotlin\random\FallbackThreadLocalRandom$implStorage$1.java**
12.  **org\openbot\vehicle\Noise.java**

## Remediation :

It is recommend to Use java.security.SecureRandom class for random number generation.

Severity : Medium

## Proof Of Concept

![OpenBot_Insufficient_Random_ActivityResultRegistry-1](https://github.com/ctflearner/Android_Findings/assets/98345027/2aa2088c-b57b-4510-a975-dd2bd03a5b2a)

![OpenBot_Insufficient_Random_DNS-6](https://github.com/ctflearner/Android_Findings/assets/98345027/e0068848-9921-4271-b4a2-68db6a86866e)

![OpenBot_Insufficient_Random_FileCache-7](https://github.com/ctflearner/Android_Findings/assets/98345027/3ac94d53-c04a-4a49-8d6c-49a81bf5f06c) 

![OpenBot_Insufficient_Random_Gauge-3](https://github.com/ctflearner/Android_Findings/assets/98345027/a311eb0d-4ed7-4c22-a070-aeb2fb990f56) 

![OpenBot_Insufficient_Random_Handshake-5](https://github.com/ctflearner/Android_Findings/assets/98345027/bfe2566d-bbd1-4a09-9dda-8d0941797c3b)

![OpenBot_Insufficient_Random_inlinedletlambda-9](https://github.com/ctflearner/Android_Findings/assets/98345027/7d076f8b-8146-43ac-9df0-13cadb4d56d2) 

![OpenBot_Insufficient_Random_MultipartEntityBuilder_10](https://github.com/ctflearner/Android_Findings/assets/98345027/618b2d0d-aad3-44de-892c-f84d3edb177a) 

![OpenBot_Insufficient_Random_Noise-12 1](https://github.com/ctflearner/Android_Findings/assets/98345027/1c8a9638-d01a-4a96-8d51-4e8da0662924) 

![OpenBot_Insufficient_Random_Noise-12](https://github.com/ctflearner/Android_Findings/assets/98345027/c110349a-e0e6-4531-88a0-72852a6ac506) 

 ![OpenBot_Insufficient_Random_RandomCompat-2](https://github.com/ctflearner/Android_Findings/assets/98345027/bddbad68-04ab-4fac-8e88-953aa86104de)

 ![OpenBot_Insufficient_Random_RtmpConnection_4 1](https://github.com/ctflearner/Android_Findings/assets/98345027/6cca3843-d02c-4c71-acc1-ecf54fc862b1) 

 ![OpenBot_Insufficient_Random_RtmpConnection_4](https://github.com/ctflearner/Android_Findings/assets/98345027/37d774ba-e254-4a48-bb0d-6140c0085f04) 

 ![OpenBot_Insufficient_Random_SimpleMultipartEntity_8](https://github.com/ctflearner/Android_Findings/assets/98345027/129cd9c9-d16d-46f3-abf5-8de78f9ab676) 

 ![OpenBot_Insufficient_Random_Threadlocalrandom_11](https://github.com/ctflearner/Android_Findings/assets/98345027/abeccdec-d3b4-4eb2-9407-1d4978a73945)














