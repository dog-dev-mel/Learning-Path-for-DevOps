# Reversible encryption
Storing encrypted passwords in a way that is reversible means that the encrypted passwords can be decrypted. A knowledgeable attacker who is able to break this encryption can then log on to network resources by using the compromised account.

It includes **symmetrical encryption** and **asymmetrical encryption**.


## **symmetrical encryption**
This is the simplest kind of encryption that involves only one secret key to cipher and decipher information. Symmetric encryption is an old and best-known technique. It uses a secret key that can either be a number, a word or a string of random letters. It is a blended with the plain text of a message to change the content in a particular way. The sender and the recipient should know the secret key that is used to encrypt and decrypt all the messages. Blowfish, AES, RC4, DES, RC5, and RC6 are examples of symmetric encryption. The most widely used symmetric algorithm is AES-128, AES-192, and AES-256.

The main disadvantage of the symmetric key encryption is that all parties involved have to exchange the key used to encrypt the data before they can decrypt it.


# Does Irreversible encryption exist?
Encryption, by its very definition is reversible, so there is no such thing as irreversible encryption, in the same way there are no dogs which are also cats.

There are other mathematical processes which are irreversible though - properly speaking, these are not called encryption, **they are called hashing algorithms such as MD5, SHA-1, SHA-2, NTLM, and LANMAN**.

A chinese reseracher(IACR Fellow Xiao-yun Wang) has proposed a method to get same MD5 value for different Plaintext.
MD5(M1)=MD5(M2)

Other explanation about Irreversible encryption:
A cryptographic process that transforms data deterministically to a form from which the original data cannot be recovered, even by those who have full knowledge of the method of encryption. The process may be used to protect stored passwords in a system where the password offered is first encrypted before it is matched against the stored encrypted password. Illegal access to the stored password therefore does not permit access to the system.

https://www.ssl2buy.com/wiki/symmetric-vs-asymmetric-encryption-what-are-differences
https://zhuanlan.zhihu.com/p/30573146
https://www.cnblogs.com/luminji/archive/2011/06/01/2065438.html
