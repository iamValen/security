## Hashes
#### Represent data as a short string of text
- A message digest, a fingerprint
#### One-way trip
- Impossible to recover the original message from the digest
- Used to store passwords / confidentiality
#### Verify a downloaded document is the same as the original
- Integrity
#### Can be a digital signature
- Authentication, non-repudiation, integrity


## Hash Example
#### SHA256 hash
- 256 bits / 64 hexadecimal characters
#### My name is Professor Messor.
- SHA256 hash: 19da9a2e26f3bff67f0522f...
#### My name is Professor Messor!
- SHA256 hash: 54381cae1eea10892d81c8...
#### One change makes the hash very different


## Collision
#### Hash functions
- Take an input of any size
- Create a fixed size string
- Message digest, checksum
#### The hash should be unique
- Different inputs should never create the same hash
- If they do, it's a collision
#### MD5 has a collision problem
- Found in 1996
- Don't use MD5 for anything important


## Practical Hashin
#### Verify a downloaded file
- Hashes may be provided on the download site
- Compare the downloaded file hash with the posted hash value
#### Password storage
- Instead of storing the password, store a salted hash
- Compare hashes during the authentication process 
- Nobody knows the password stored


## Adding some salt
#### Salt
- Random data added to a password when hashing
#### Every user gets their own random salt
- The salt is commonly stored with the password
#### Rainbow tables won't work with salted hashes
- Rainbow tables is a pre-compiled of every possible input and every hash for it
- Additional random value added to the original
#### This slows things down the brute force process
- It doesn't completely stop the reverse engineering


## Digital Signature
#### Prove the message was notchanged
- Integrity
#### Prove the source of the message
- Authentication
#### Make sure the signature isn't fake
- Non-repudiation
#### Sign with the private key
- The message doesn't need to be encrypted
- Nobody else can sign this (obviously)
#### Verify with the public key
- Any change in the message will invalidate the signature