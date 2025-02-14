# Goodreads: Book Reviews 

## Project-Details
```
Application Name: Goodreads: Book Reviews
Version:2.31.0
Package Name: com.goodreads
Build: 18 (1080894510)
Google Play Store-link:  https://play.google.com/store/apps/details?id=com.goodreads&hl=en_IN 
```
## TITLE : Hardcoded Password Found in APK Source Code

## Description:

A security vulnerability has been identified in the Goodreads: Book Reviews Android application (Version 2.31.0, Build 18). 
The APK source code contains hardcoded passwords in multiple locations. These credentials are exposed upon decompilation, 
allowing potential attackers to access sensitive application resources.

CWE-798: Use of Hard-coded Credentials

**Impact:**

- **Unauthorized Access:** Attackers can extract the hardcoded credentials and use them to gain unauthorized access to backend systems, APIs, or databases.

### **Recommended Mitigation:**

- Remove all hardcoded passwords from the source code.

### Associated Files

1. **com\amazon\identity\auth\device\api\MAPAccountManager.java**
2.  **com\amazon\kindle\restricted\webservices\grok\GrokServiceConstants.java**
3. **com\amazonaws\mobile\auth\userpools\CognitoUserPoolsSignInProvider.java**
4. **com\amazonaws\mobile\client\AWSMobileClient.java**
5. **com\amazonaws\mobileconnectors\cognitoidentityprovider\util\CognitoServiceConstants.java**
6. **com\github\scribejava\core\model\OAuthConstants.java**
7. **com\goodreads\android\facebook\GoodreadsFacebookClientImpl.java**
8. **com\goodreads\android\lwa\GoodreadsLWAClientImpl.java**
9. **com\goodreads\kindle\application\Constants.java**

## Proof of Concept(PoCs)
- Navigate to the Affected location and search for "password" .

![hardcoede-1](https://github.com/user-attachments/assets/da21340d-f946-44f2-aa5f-2a8b982932b1)

![hardcoede-2](https://github.com/user-attachments/assets/acabf44a-abf3-4739-be43-8b13a726ec65)


