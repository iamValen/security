## Open permission
#### Very easy to leave a door open
- The hackers will always find it
#### Increasingly common with cloud storage
- Statistical chance of finding an open permission
#### June 2017 - 14 million Verizon records exposed
- Third-party left an Amazon S3 data repository open
- Researcher found the data before anyone else
#### Secure your permission!


## Unsecured Admin Accounts
## The Linux root account
- The windows Administrator or superuser account
#### Can be a misconfiguration
- Intentionally configuring an easy-to-hack password
- 123456, ninja, football
#### Disable direct login to the root account
- Use the su or sudo option
#### Protect accounts with root or administrator access
- There should be not a lot of these


## Insecure Protocols
#### Some protocols aren't encrypted
- All traffic sent in the clear
- Telnet, FTP, SMTP, IMAP...
#### Verify with a packet capture
- View everything sent over the network
#### Use the encrypted version
- SSH, SFTP, IMAPS, HTTPS, etc.


## Default Settings
#### Every application and network device has a default login
- Not all of these are ever changed
#### Mirai botnet
- Takes advantage of default configurations
- Takes over Internet of Things devices
- 60+ default configurations
- Cameras, routers, doorbells, garage door openers, etc.
#### Mirai released as open-source software
- There's a lot more where that came from


## Open ports and services
#### Services will open ports
- It's important to manage access
#### Often managed with a firewall
- Manage traffic flows
- Allow or deny based on port number or application
#### Firewall rulesets can be complex
- It's easy to make mistakes
#### Always test and audit
- Double and triple check