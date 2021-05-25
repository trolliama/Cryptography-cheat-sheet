# PGP
 Pretty Good Privacy is an encryption software which provides security, privacy and authentication to online communication systems. 
 It is most widely used in email encryption system because of your privacy and security level. When you send an email using PGP no one 
 can read it unless you provide the session key.

## History
  Phil Zimmerman was the first person to create a PGP software encryption and according to him the program was made available free of charge due
  to a growing social demand for privacy.
  
  Before PGP, your Internet provider, your email provider, hackers, or the government could theoretically read your messages. PGP was 
  developed in the 1990s to allow email and other types of messages to be exchanged privately. Today, PGP has been standardized into OpenPGP, 
  enabling anyone to write PGP software that is compatible and interoperable with other implementations. Several OpenPGP-compliant developer 
  libraries have been created to help programmers implement PGP encryption in their applications

## How it works
  This model of encryption uses both symmetric and asymmetric encryption to achieve high levels of security and privacy. let's look to the 
  diagram and get a better understanding of the process.
  
  ![alt text][logo]

  [logo]: https://i.imgur.com/ouXKUpX.png "PGP encryption Process by ProtonMail"
  
  ### PGP encryption
   Here the encription it's made by a symetric process. First the PGP will create a session key which is an enormous number and is used only once. This sesion key 
   will be used to encrypt the content of the message (most programs will compress the message before the encryption).
   
   Such a key is generated randomly through a symmetric encryption system and each PGP communication session has a single session key.
   
   The session key and the encrypted message now need to be sent to the recipient. For acomplish this in a secure way the session key is encrypted with the 
   public key of the recipient and sent to him with the encrypted message. So because the only feasible way to decrypt the session key is using the recipient private 
   key, the message is sent securely
   
   In the reipient side the session key is decrypted with his private key and then used to decrypt the message. Simple rigth?
 
   > The use of a session key to encrypt the message and not a public key directly it's because the public key have an asymetric cryptography process 
   > which is much slower than a symetric one, so would be inconvenient to use this to encrypt a large amount of text or files
  
  ### Digital Signatures
  A digital signature proves to the recipient that no one has manipulated the message or the sender in some how. The way that it's made it's using a combination 
  of the sender private key and a mathematical redux (message digest) of the plaintext message. This combination will generate an unique number known as the 
  digital signature



## References
- [ProtonMail Blog Post](https://protonmail.com/blog/what-is-pgp-encryption/)
- [Binance Academy Blog Post](https://academy.binance.com/en/articles/what-is-pgp)
