# Elliptic Curve Integrated Encryption Scheme (ECIES)

## What is a Elliptic Curve Integrated Encryption Scheme
Elliptic Curve Integrated Encryption Scheme, or ECIES, is a hybrid encryption system proposed by Victor Shoup in 2001. ECIES combines a Key Encapsulation Mechanism (KEM) with a Data Encapsulation Mechanism (DEM). The system independently derives a bulk encryption key and a MAC key from a common secret. Data is first encrypted under a symmetric cipher, and then the cipher text is MAC'd under an authentication scheme. Finally, the common secret is encrypted under the public part of a public/private key pair.

## Why would I want to use ECC?
The small key sizes make ECC very appealing for devices with limited storage or processing power, which are becoming increasingly common in the IoT. A 256 bit ECC key is equivalent to RSA 3072 bit keys (which are 50% longer than the 2048 bit keys commonly used today). In terms of more traditional web server use cases, the smaller key sizes can offer speedier SSL handshakes (which can translate to faster page load times) and stronger security.


## ecies.py
The goal for this script is to provde some easy understanding to how ecies work. By creating two sets of key pairs (receiver and sender). By using (ECDH) we create a shared secret between the sender and receiver that allows them to communicate with eachother without anyone being able to read their messages. The user can also store their shared secret to a hidden file, and load the secret key the next time they run the script.

Before you try to use the program I would highly recommend you to read the following links: 
https://en.wikipedia.org/wiki/Elliptic-curve_Diffie%E2%80%93Hellman
https://www.cryptopp.com/wiki/Elliptic_Curve_Integrated_Encryption_Scheme
https://en.wikipedia.org/wiki/Diffie%E2%80%93Hellman_key_exchange#Secrecy_chart
## TODO
- store keys to file (maybe with password)
 
 ## Flow diagram 
 ![alt text](https://github.com/gudbrandsc/ECIES-project/blob/master/1_A3yiRaX7xBPBsovR_NyuVQ.png "Logo Title Text 1")

