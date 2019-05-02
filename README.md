# Elliptic Curve Integrated Encryption Scheme (ECIES)

## What is a Elliptic Curve Integrated Encryption Scheme
Elliptic Curve Integrated Encryption Scheme, or ECIES, is a hybrid encryption system proposed by Victor Shoup in 2001. ECIES combines a Key Encapsulation Mechanism (KEM) with a Data Encapsulation Mechanism (DEM). The system independently derives a bulk encryption key and a MAC key from a common secret. Data is first encrypted under a symmetric cipher, and then the cipher text is MAC'd under an authentication scheme. Finally, the common secret is encrypted under the public part of a public/private key pair.

## Why would I want to use ECC?
The small key sizes make ECC very appealing for devices with limited storage or processing power, which are becoming increasingly common in the IoT. A 256 bit ECC key is equivalent to RSA 3072 bit keys (which are 50% longer than the 2048 bit keys commonly used today). In terms of more traditional web server use cases, the smaller key sizes can offer speedier SSL handshakes (which can translate to faster page load times) and stronger security.


## Install python ECIES
I was unable to use the ecies library after running.
``` 
pip install eciespy
```
I therefor decided to follow some examples that I found online for key generation, encryption and decryption. To see the result of this program check this esies.py. 

## TODO
- Add ui to display keys 
- store keys to file (maybe with password)
 
 ## Flow diagram 
 ![alt text](https://github.com/gudbrandsc/ECIES-project/blob/master/1_A3yiRaX7xBPBsovR_NyuVQ.png "Logo Title Text 1")

