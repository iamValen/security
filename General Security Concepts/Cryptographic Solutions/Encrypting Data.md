## Encrypting stored data
#### Protect data on storage devices
- SSD, hard drive, USB drive, cloud storage, etc.
- This is data at rest
#### Full-disk and partition/volume encryption
- BitLocker, FileVault, etc.
#### File encryption
- EFS (encrypting file system), third-party utilities


## Database encryption
#### Protecting stored data
- And the transmission of that data
#### Transparent encryption
- Encrypt all database information with a symmetric key
#### Record-level encryption
- Encrypt individual columns
- Use separate symmetric keys for each columns


## Transport Encryption
#### Protect data traversing the network

#### Encrypting in the application
- Browsers can communicate using HTTPS
#### VPN (Virtual Private Network)
- Encrypts all data transmitted over the network, regardless of the application
- Client-based VPN using SSL/TLS
- Site-tosite VPN using IPsec


## Encryption algorithms
#### There are many, many different ways to encrypt data
- The proper "formula" must be used during encryption and decryption
#### Both sides decide on the algorithm before encrypting the data
- The details are often hidden from the end user
#### There are advantages and disadvantages between algorithms
- Security level, speed, complexity of implementation, etc.


## Cryptographic Keys
#### There's very little that isn't known about the cryptographic process
- The algorithm is usually a known entity
- The only thing you don't know is the key
#### The key determines the output
- Encrypted data
- Hash value
- Digital signature
#### Keep your key private
- It's the only thing protecting your data


## Key lengths
#### Larger keys tend to be more secure
- Prevent brute-force attacks
- Attackers can try every possible key combination
#### Symmetric encryption
- 128-bit or larger symmetric keys are common
- These numbers get larger and larger as time goes on
#### Asymmetric encryption
- Complex calculations of prime numbers
- Larger keys than symmetric encryption
- Common to see key length of 3,072 bits or larger


## Key stretching
#### A weak key is a weak key
- By itself, it's not very secure
#### Make a weak key stronger by performing multiple processes
- Hash a password. Hash the hash of the password. And continue...
- Key stretching, key strengthening
#### Brute force attacks would require reversing each of those hashes
- The attacker has to spend much more time, even though the key is small
