# NETWORK NOTES 

## UNMISSABLE PROTOCOLS
protocol {prot number} : description
> - FTP {21} : File Transfert Protocol. Protocol to share files between a client and a serveur.  
> - SSH {22} : Secure Shell. Securised way to login to a remote device.
> - HTTP {80} : HyperText Transfer Protocol. Client-server data exchange using the World Wide Web.
> - HTTPs {443} : same as HTTP with TLS certificat to ensure authentification  and confidentiality.
> - SMB {445} : Server Message Block. Same as FTP but share also print devices (vuln source)
> - RDP {3389} : Remote Desktop Protocol

## VPN (VIRTUAL PRIVATE NETWORK)
Simulate that devices from 2 networks are in the same network. Provides encryption to assure confidentiality of the datas.

There are 3 types of VPN:
> PPP : Point To Point protocole, assures encryption but not routable in internet.  
> PPTN: Point to Point Tunneling Protocol. Allows data from PPP to be routed in internet.  
> IPsec : Internet Security Protocol. Encrypts data using the Internet Protocol framework.