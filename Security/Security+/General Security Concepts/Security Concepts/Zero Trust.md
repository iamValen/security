# Many networks are relatively open on the inside
- Once you're through the firewall, there are few security controls
# Zero trust is a holistic approach to network security
- Covers every device, every process, every person
# Everything must be verified
- Nothing is inherently trusted
- Multi-factor authentication, encryption, system permission, additional firewalls, monitoring and analytics, etc.


## Planes of Operation
#### Split the network into functional planes
- Applies to physical, virtual, and cloud components
#### Data plane
- Process the frames, packets, and network data
- Processing, forwarding, trunking, encrypting, NAT
#### Control plane
- Manages the actions of the data plane
- Define policies and rules
- Determines how packets should be forwarded
- Routing tables, session tables, NAT tables


## Controlling trust
#### Adaptive identity
- Consider the source and the requested resources
- Multiple risk indicators - relationship to the organization, physical location, type of connection, IP/Mac address, etc.
- Make the authentication stronger, if needed
#### Threat scope reduction
- Decrease the number of possible entry points
#### Policy-driven access control
- Combine the adaptive identity with a predefined set of rules


## Security zones
#### Security is more than a one-to-one relationship
- Borad categorizations provide a security-related foundation
#### Where are you coming from and where are you going
- Trusted, untrusted
- Internal network, external network
- VPN 1, VPN5, VPN 11
- Marketing, IT, Accounting, etc.
#### Using the zones may be enough by itself to deny access
- For example, **Untrusted** to **Trusted** zone traffic
#### Some zones are implicitly trusted
- For example, **Trusted** to **Internal** zone traffic


## Policy enforcement point
#### Subject and systems
- End users, applications, non-human entities
#### Policy enforcement point (PEP)
- The gatekeeper
#### Allow, monitor, and terminate connections
- Can consist of multiple components working together

![[Pasted image 20251012154935.png]]

But it doesn't provide the decision if the traffic is allowed or disallowed


## Applying trust in the planes
#### Policy Decision Point
- There's a process for making an authentication decision
#### Policy Engine
- Evaluates each access decision based on policy and other information sources
- Grant, deny or revoke
#### Policy Administrator
- Communicates with the Policy Enforcement Point
- Generates access tokens or credentials
- Tells the PEP to allow or disallow access

![[Pasted image 20251012155238.png]]