## XSS
- Cascading Style Sheets (CSS) are other thing so we use XSS
#### Originally called cross-site because of browser security flaws
- Information from one site could be shared with another
#### One of the most common web vulnerabilities
- Takes advantage of the trust a user has for a site
- Complex and varied
#### XSS commonly uses JavaScript
- Do you allow scripts? 

![[Pasted image 20251029213433.png]]


## Non-persistent (reflected) XSS attack
#### Web site allows scripts to run in user input
- Search box is a common source
#### Attacker emails a link that takes advantage of this vulnerability
- Runs a script that sends credentials/session IDs/cookies to the attacker
#### Script embedded in URL executes in the victim's brower
- As if it came from the server
#### Attacker uses credentials/session IDs/cokkies to steal victim's information without their knowledge
- Very sneaky


## Persistent (stored) XSS attack
#### Attacker posts a message to a social network
- Includes the malicious payload
#### It's now "persistent"
- Everyone gets the payload
#### Not specific target
- All viewers to the page
#### For social networking, this can spread quickly
- Everyone who views the message can have it posted to their page
- Where someone else can view it and propagate it further...


## Hacking Subaru
#### In June 2017, Aaron Guzman
- Security researcher
#### When authenticating with Subaru, users get a token
- That never expires (very bad!)
#### A valid token allowed any service request
- Even adding your email address to someone else's account
- Now you have full access to someone else's car
#### Web front-end included an XSS vulnerability
- A user clicks a malicious link, and you have their token


## Protecting against XSS
#### Be careful when clicking untrusted links
- Never blindly click in your email inbox. Never
#### Consider disabling JavaScript
- Or control with an extension
- This offers limited protection
#### Keep your browser and applications updated
- Avoid the nasty browser vulnerabilities
#### Validate input
- Don't allow users to add their own scripts to an input field