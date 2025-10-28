#### A method used by the attacker
- Gain access or infect to the target
- Also called "attack vectors"
#### A lot of work goes into finding vulnerabilities in these vectors
- Some are more vulnerable than others
#### IT security professional spend their career watching these vectors
- Protect existing vectors
- Find new vectors


## Message-based vectors
#### One of the biggest (and most successful) threat vectors
- Everyone has at least one of these messaging systems
#### Email
- Malicious links in an email
- Link to malicious sits
#### SMS (Short Message Service)
- Attacks in a text message


#### Phishing attacks
- People want to click links
- Links in an email, links send via text or IM
#### Deliver the malware to the user
- Attach it to the email
- Scan all attachments, never launch untrusted links
#### Social engineering attacks
- Invoice scams
- Cryptocurrency scams


## Image-based vectors
#### Easy to identify a text-based threat
- It's more difficult to identify the threat in an image
#### Some image formats can be a threat
- The SVG ( Scalable Vector Graphic) format
- Image is described as XML (Extensible Markup Language)
#### Significant security concerns
- HTML inkection
- Javascript attack code
#### Browsers must provide input validation
- Avoids running malicious code

![[Pasted image 20251022185921.png]]

## File-based vectors
#### More than just executables
- Malicious code can hide in many places
#### Adobe PDF
- A file format containing other objects
#### ZIP/RAR files (or any compression type)
- Contains many different files
#### Microsoft Office
- Documents with macros
- Add-in files


## Voice call vectors
#### Vishing (Voice Phishing)
- Phishing over the phone 
#### Spam over IP
- Large-scale phone calls
#### War dialing
- Instances where attackers trying to find unpublished numbers to get access to systems
#### Call tampering
- Disruption voice calls


## Removable device vectors
#### Get around the firewall
- The USB interface
#### Malicious software on USB flash drives
- Infect air gapped networks
- Industrial systems, high-end security services
#### USB devices can act as keyboards
- Hacker on a chip
#### Data exfiltration
- Terabytes of data walk out the door
- Zero bandwidth used


## Vulnerable software vectors
#### Client-based
- Infected executable
- Known (or unknown) vulnerabilites
- May require constant updates
#### Agentless
- No installed executable
- Compromised software on the server would affect all users
- Client runs a new instance each time


## Unsupported system vectors
#### Patching is an important prevention tool
- Ongoing security fixes
#### Unsupported systems aren't patched
- There may not even be an option
#### Outdated operating systems
- Eventually, even the manufacturer won't help
#### A single system could be an entry
- Keep your inventory and records current


## Unsecure network vectors
#### The network connects everything 
- Ease of access for the attackers
- View all (non-encrypted) data
#### Wireless
- Outdated security protocols (WEP, WPA, WPA2)
- Open or rogue wireless networks
#### Wired
- Unsecure interfaces - No 802.1X -> auth protocol that prevents anyone from gaining access to the network unless you provide the proper credentials
#### Bluethooth
- Reconnaissance - to see where a particular system might be
- Implementation vulnerabilities


## Open service ports
#### Most network-based services connect over a TCP or UDP port
- An "open" port
#### Every open port is an opportunity for the attacker
- Application vulnerability or misconfiguration
#### Every application has their own open port
- More services expand the attack surface
#### Firewall rules
- Must allow traffic to an open port


## Default credentials
#### Most devices have default usernames and password
- Change yours!
#### The right credentials provide full control
- Administrator access
#### Very easy to find the defaults for your access point or router
- https://www.routerpasswords.com


## Supply chain vectors
#### Tamper with the underlying infrastructure
- Or manufacturing process
#### Managed services providers (MSPs)
- Access many different customer networks from one location
#### Gain access to a network using a vendor
- 2013 Target credit card breach
#### Suppliers
- Counterfeit networking equipment
- Install backdoors, substandard performance and availability
- 2020 - Fake Cisco Catalyst Switches