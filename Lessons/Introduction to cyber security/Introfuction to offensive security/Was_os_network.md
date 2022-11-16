# WEB APPLICATION SECURITY

## RISKS
**Broken access control**
> access control means that users have legitimate files access permissions. If it is not well configured it is a vulnerability.

**Identification and authentification failure**
> We have to prevent attackers to bruteforce passwords, users to store weak passwords and not strongly encrypted.

**Injection**
> User input may be use to inject malicious code and lead to anormal behavior of the web site.

**Cryptographic Failures**
> Weak cryptographic algorithms and secret...

***
## Keywords
**IDOR** : Insecure Direct Object Reference

# OS

## Autehntification and weak passwords
**NCSC**: Ntaional cyber security center
> Publied the 100 000 most used password https://www.ncsc.gov.uk/blog-post/passwords-passwords-everywhere

We shouldn't use weak (common password) and reuse it in several website. Because if a website is compromised then your password will be leaked...

***
## history
>Linux command that show all the previous commands used. If user type his password while using su (he fails) you can see it.

# Network security
**Hardware appliance**
>- Firewall
>- IDS : intrusion dectection system. Detects intrusions.
>- IPS : intrusion prevention system. Tires to block detected network intrusions.

**software security solutions**
>- antivirus : detects malicious files and block them from executiong.
>- host firewall : sofware version of firewall, local to the machine.  

***
## KILL CHAIN
Lockheed Martin defined  several steps to atteck a system:   
1. **Recon** : reconaissance, the attacker tries to get as much as possible about the target like for example the IP addresses, types of servers, operating system, name of users, emails.
2. **weaponization**: prepare a file with walicious script, remote access.
3. **delivery**: delivering the weaponized file to the target with for exemple email, usb flash memory.
4. **exploitation**: when the user open the malicious file then the filesystem is corrupted.
5. **installation**: thanks to the previous step, the malware is now installed on the targeted system and the attacker has an access to the system.
6. **Command and control**: the malware provides to the attacker a control ability over the system.
7. **actions on objectives**: the attacker does what he wants, like data exfiltration or cyphering.

Litle example (easy) of the kill chain :
- Using **Nmap** to the targeted machine to know what ports is open, protocols used. 
- We see that FTP is open, we connect to the server using the "anonymous" login (real vulnerability).
- with the ls command we can list the files on the server and download them with **get filename** command.
- we get a secret key that allows us to connect (ssh) to the remote server with root account and see the exercice's flag.
- We don't exploit extraction or stealth.