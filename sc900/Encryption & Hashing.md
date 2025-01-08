## Symmetric and Asymmetric Encryption
![Diagram showing the concept of symmetric and asymmetric encryption.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-security-concepts-methodologies/media/6-encryption.png)
1. Symmetric: uses the same key to encrypt and decrypt
2. Asymmetric: uses a public and private key pair
- Either key can encrypt data but the key used cannot be used to decrypt encrypted data.
	- to decrypt you would need a paired key.
### Encryption for data at rest
- data that is stored on a physical device such as a server. It may be stored in a database or a storage account
### Encryption for data in transit
- data moving from one location to another, such as across the internet or through a private network.
### Encryption for data in use
- securing data in nonpersistent storage (RAM or CPU caches)

# [[Hashing]]
- uses an algorithm to convert text
	- each time the same text is hashed using the same algorithm, the same hash value is produced. That hash can then be used as a unique identifier of its associated data
- [[Hashing]] doesn't use keys compared to [[encryption]]
