Asymmetric encryption was developed in the 1970s. It addresses the secure distribution and proliferation of keys that are associated with symmetric encryption.

Asymmetric encryption changed the way cryptographic keys were shared. Rather than one encryption key, an asymmetric key is composed of two elements, a **private key** and a **public key**, which form a **key pair**. The public key, as the name suggests, can be shared with anyone, so individuals and organizations don’t need to worry about its secure distribution.

The private key must be kept safe. It's looked after only by the person who generated the key pair and isn't shared with anyone. A user who needs to encrypt a message would use the public key, and only the person holding the private key could decrypt it.![This diagram shows the creation of a key pair and how you can share the public key, but need to keep the private key safe.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-concepts-of-cryptography/media/key-pair-generation.png)
Asymmetric encryption, with its use of public and private keys, removes the burden of secure distribution of keys. This concept also addresses the proliferation of keys we saw in symmetric encryption. Consider the example of the government-based organization with 1,000 employees, where each individual must be able to communicate securely. With asymmetric encryption, every person will generate a key pair, resulting in 2,000 keys. With symmetric encryption, this would have required 450,000 keys.
## Asymmetric encryption
While the algorithms and mathematics that underpin asymmetric encryption are complex, the principle of how it works is relatively easy.

Let's assume that we have two people, Quincy and Monica, who need to communicate securely and privately. Using readily available software tools, Quincy and Monica each create their own key pair.

The first thing that Quincy and Monica will do is share their **public keys** with each other. Because public keys aren't secret, they can exchange them via email.![This diagram shows how Quincy must share his public key with Monica so she can send him ciphertext. It also slows Monica sharing her public key with Quincy.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-concepts-of-cryptography/media/asymmetric-public-key-sharing.png)
When Quincy wants to send a secured message to Monica, he uses her **public key** to encrypt the [[plaintext]] and create the [[ciphertext]]. Quincy then sends the [[ciphertext]] to Monica using whatever means he wants, such as email. When Monica receives the [[ciphertext]], she uses her **private key** to decrypt it, turning it back to [[plaintext]].![This diagram shows the process of encrypting a message using Monica’s public key, and Monica decrypting the ciphertext using her private key.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-concepts-of-cryptography/media/asymmetric-encryption-process.png)
When Monica wants to respond, she uses Quincy's **public key** to encrypt the message before sending it. Quincy then uses his **private key** to decrypt it.

Let's assume that Eve is interested in what Quincy and Monica are saying. Eve intercepts a [[ciphertext]] message sent from Quincy to Monica. Additionally, Eve knows Monica's public key.

Because Eve doesn’t know Monica’s private key, she has no way of decrypting the [[ciphertext]]. If Eve tries to decrypt the [[ciphertext]] with Monica’s public key, she will see gibberish.

Given the nature of asymmetric encryption, even if you know the public key, it's impossible to discover the private key.
