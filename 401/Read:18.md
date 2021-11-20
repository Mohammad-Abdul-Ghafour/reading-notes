# Cryptography

**`cryptography`** is a package which provides cryptographic recipes and primitives to Python developers.

cryptography includes both high level recipes and low level interfaces to common cryptographic algorithms such as symmetric ciphers, message digests, and key derivation functions.

## Encryption :

**`Encryption`** involves converting human-readable plaintext into incomprehensible text, which is known as ciphertext.

Essentially, this means taking readable data and changing it so that it appears random.

**`Encryption`** involves using a cryptographic key, a set of mathematical values both the sender and recipient agree on.

It helps protect private information, sensitive data, and can enhance the security of communication between client apps and servers.

![Encryption](https://miro.medium.com/max/1000/0*jR2uHh4xddtkP_RU.png)

## Decryption :

**`Decryption`** is a process that transforms encrypted information into its original format.

The process of encryption transforms information from its original format — called plaintext — into an unreadable format — called ciphertext — while it is being shared or transmitted.

To do this, parties to a private conversation use an encryption scheme, called an algorithm, and the keys to encrypt and decrypt messages. (Encrypted messages are called ciphertext, as algorithms are also called ciphers.)

Message recipients decrypt the information back into its original, readable format. Future messages when passed through the system are encrypted, and vice versa.

It is required for several security-related actions, including threat prevention, advanced malware prevention, file blocking, data filtering and blocking of malicious web and application traffic.

## Cracking the cipher :

uncovering the original data without knowing the secret, by using a variety of clever techniques called **`Cracking`**.

There are three main techniques he could use :

* frequency analysis.
* known plaintext.
* brute force.

## Caesar Cipher :

The **`Caesar Cipher`** technique is one of the earliest and simplest method of encryption technique.

It’s simply a type of substitution cipher, i.e., each letter of a given text is replaced by a letter some fixed number of positions down the alphabet.

For example with a shift of 1, A would be replaced by B, B would become C, and so on. The method is apparently named after Julius Caesar, who apparently used it to communicate with his officials. 

Thus to cipher a given text we need an integer value, known as shift which indicates the number of position each letter of the text has been moved down.

The encryption can be represented using modular arithmetic by first transforming the letters into numbers, according to the scheme, A = 0, B = 1,…, Z = 25. Encryption of a letter by a shift n can be described mathematically as.

> E_n(x)=(x+n)mod\ 26 *`(Encryption Phase with shift n)`*

> D_n(x)=(x-n)mod\ 26 **`(Decryption Phase with shift n)`**

![Caesar Cipher](https://cdn.guru99.com/images/2/cipher-cryptography.png)

![Types of Cipher](https://cdn.educba.com/academy/wp-content/uploads/2019/10/Types-of-Cipher.png)