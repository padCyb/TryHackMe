# WINDOWS FUNDAMENTALS

**Bitlocker** : Encryption service of the pro licence edition, when the device is lost or stolen everything is encrypted.

**NTFS** : New Technology File System. Windows-s actual file system, it contains a system journal, allows permissions on files and permits ELF (Encrypted File System).

The OS can be found is C:\Windows. The respective env var is %windir%  

>In the run box : lusrmgr.msc  
>Account (and permissions) manager

**UAC** : User Account Control
>In the past most of people are connected to their computer with administrator account, it was risquy because it simplifies the work for a malware if it has access to an account with hight priviligies.  
>This is why since windows vista everyone is connected with a user account and get temporary access to the admin account when it's needed. This service is possible thanks to UAL.

**VSS**: Volume Shadow Copy Service.
>Performs a snapshot of the selected disk in order to hav e a backup.  
>Most of the time, malwares know where to find the backups and delete them. The solution is to store the backup outside the computer.  

**msconfig**: System configuration utility. It is a program that monitor the startup application and services.  
>We won't explicitely tells to the system what application has to be lunch at boot but we can access to the management panel from this app (redirect to task manager). Useful to see all services configured of the PC.

**msinfo32**: System information.
> Huge source of info from hardware stats, drivers to sofware installed. We can have network info and error reports aswell.

**compmgmt.msc**: Computer Management
> Manage file system contents, task scheduler, disk management...

**remon**: Ressource monitor
>    CPU,
    Disk,
    Network,
    Memory.  
    The network panel is very interesting, we can see real-time load, opened ports ...

**command prompt**
> "cmd" /> \# display help manual of the cmd.  
cls \# clear the shell.  
netstat \# network protocol statistics tool.  
net \# ressources management (network, user etc...). net help to see the options.

**List of CMD commands**: https://ss64.com/nt/

**regedt32** : edit the windows registry informations
> https://learn.microsoft.com/en-us/troubleshoot/windows-server/performance/windows-registry-advanced-users


---
## MITRE VULN EXPLOIT 
Living Off The Land exploits : being undetected while executing scripts or files transfer.

https://lolbas-project.github.io/#