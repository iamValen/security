# Authentication, Authorization, and Accounting

### Identification
- Who you claim to be
- Usually your username
### Authentication
- Prove you are who you say who you are
- Password and other auth factors
### Authorization
- Based on your identification and authentication, what access do you have?
### Accounting
- Resources used: Login time, data sent and received, logout time

# Practical use

![[Pasted image 20251012131258.png]]

# Authenticating systems
### You have to manage many devices
- Often devices that we'll never physically see
### A system can't type a password
- And you may not want to store one
### How can you truly authenticate a device
- Put a digitally signed certificate on the device
### Other business processes rely on the certificate
- Access to the VPN from authorized devices
- Management software can validate the end device

## Certificate authentication
- An organization has a trusted **Certificate Authority **(CA)
- The organization creates a certificate for a device and digitally signs the certificate with the organization's CA
- The certificate can now be included on a device as an authentication factor

# Authorization models
#### The user or device has now authenticated
- To what do they now have access?
- Time to apply an authorization model
#### Users and services -> data and applications
- Associating individual users to access rights does not scale
#### Put an authorization model in the middle
- Define by Roles, Organizations, Attributes, etc.

### No Authorization Model
#### A simple relationship
- User -> Resource
### Some issues with this method
- Difficult to understand why an authorization may exist
- Does not scale

### Authorization model
#### Add an abstraction
- Reduce complexity
- Create a clear relationship between the user and the resource
#### Administration is streamlined
- Easy to understand the authorizations
- Support any number of users or resources