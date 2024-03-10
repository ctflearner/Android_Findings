# Musicshelf_Manifest_Misconfiguration

Github_Repo_of_the_Project : https://github.com/KirillMakarov/Musicshelf 
--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
## Project-Details:
- Project-Name : Musicshelf
- Package-Name : com.kamakarov.musicshelf
- Version-Affected : 1.1
- Language-Used : Java
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
## Vulnerability :  Weak Hashing Algorithms 
## Description: 
It has been found that this application Musicshelf uses the SHA-1 Message_Digest Algorithm, which is weak
## Remediation: 
Use stronger hash algorithm's .
## Severity: Medium

## Location of the File  : 
File Path : io\fabric\sdk\android\services\network\PinningTrustManager.java

## Proof_Of_Concept
![Musicshelf-Weak-Hashing-Algorithm-POC-1](https://github.com/ctflearner/Android_Findings/assets/98345027/8b852dbf-b64c-40ae-8d07-10debfa44a05)
