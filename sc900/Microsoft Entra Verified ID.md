- is a managed verifiable credentials service based on open standards. [[Microsoft Entra Verified ID]] automates verifications of identity credentials & enabled privacy-protected interactions between organizations & users.
### Why do we need it?
In the digital world, transactions are increasingly done over the web & often require individuals to make claims or assertions that orgnizations can digitally verify. 
The current process obtaining & presenting a digital credential can make a verifiable claim can be difficult & cumbersome. In addition, a digital credential serves as a digital identity. 
Once you use that online digital identity to access the desired service or make an online transaction, it's common you begin to get targeted advertisements & emails for services for which you never signed up.
- That's because it's hard to retain control of your identity once you've shared it in exchange for access to a service
Individuals & businesses need a way to express their qualifications &/or personal information, that is, our digital identities, over the web in a manner that is cryptographically secure, compliant to privacy requirements, & machine readable for verification. Additionally, individuals & organizations want to be able to control how & when their digital identities are used & shared. Verifiable credentials help address these challenges
### How it works
![Diagram showing the flow for the issuance and verification of a verifiable credential.](https://learn.microsoft.com/en-us/training/wwl-sci/describe-identity-protection-governance-capabilities/media/verified-id-flow-inline.png)
- The issuer is an organization that attests to claims & grants digitally signed credentials to the user. An issuer can be an identity verification provider, a government agency, an employer, a university or any other organization that can provide proof of the user's credential
- The user receives & approves the credentials obtained from the issuer, stores & manages credentials in their digital wallet & presents it to the verifier. The credential claims are cryptographically signed with the user's private key.
- The verifier is an organization that requests proof & upon receipt, verifies that the claims in the credentials satisfy requirements. A verifier could be a prospective employer, & airline, mortgage company, or any organization that is requesting proof of the user's credential.

Supporting it all is a verifiable data registry. The underlying verifiable data registry is a collection of systems involved in creating and recording meta data that are used with verifiable credentials, including public keys. 

These systems are usually distributed networks, such as distributed ledgers, blockchains, distributed file systems, or other trusted data storage. The way to think about the verifiable data registry is as an underlying network that represents a trust system. The verifier interacts with the data registry to read the meta-data associated with the credential to then verify the credential that is presented by the user.

A common scenario with any credential is that the credential may expire, or the issuer may need to revoke that credential. The standard for verifiable credentials includes property fields in the credential to account for these scenarios.