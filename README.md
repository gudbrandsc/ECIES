# ECIES

## What is a Elliptic Curve Integrated Encryption Scheme
Elliptic Curve Integrated Encryption Scheme, or ECIES, is a hybrid encryption system proposed by Victor Shoup in 2001. ECIES combines a Key Encapsulation Mechanism (KEM) with a Data Encapsulation Mechanism (DEM). The system independently derives a bulk encryption key and a MAC key from a common secret. Data is first encrypted under a symmetric cipher, and then the cipher text is MAC'd under an authentication scheme. Finally, the common secret is encrypted under the public part of a public/private key pair.

## Install python ECIES
 - https://pypi.org/project/eciespy/
 
 ## Flow diagram 
 ![alt text](https://github.com/gudbrandsc/ECIES-project/blob/master/1_A3yiRaX7xBPBsovR_NyuVQ.png "Logo Title Text 1")

