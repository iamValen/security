### You CAN'T deny what you've said

#### It's like signing a contract
- Your signature adds non-repudiation
- You really did sign the contract
- Others can see your signature

#### Adds a different perspective for cryptography
- Proof of integrity
- Proof of origin, with high assurance of authenticity

# Proof of integrity
Using Hash can verify if the data changes, BUT doesn't necessarily associate data with an individual 

If the hash has changed the data integrity has been compromised

# Proof of origin
#### Prove the message was not changed
- Integrity
#### Prove the source of the message 
- Authentication
#### Make sure the signature isn't fake
- Non-repudiation
#### Sign with a private key
- The message doesn't need to be encrypted
- Nobody else can sign this (obviously)
#### Verify with the public key
- Any change to the message will invalidate the signature

## Creating a digital signature

![[Pasted image 20251012124948.png]]

# Verifying a digital signature

![[Pasted image 20251012125119.png]]