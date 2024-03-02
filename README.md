# Active Directory Home Lab
 A SOHO server environment connected to my network providing centralized Active Directory and Storage.

Objectives:\
Create an Active Directory environment in the Local Area Network, set up Network Attached Storage accessible to all devices, configure remote desktop for server management, enable wake on LAN for remote PC power-up, join PC into the domain, and manage users & computers.

MKtech-ADDC steps:
1.	Install Windows Server 2022
2.	Configure Windows Server 2022 (change PC-name, set static IP Address, set 127.0.0.1 as preferred DNS, set 8.8.8.8 as alternative DNS and restart the PC)
3.	Enable remote desktop in PC and configure remote desktop on PC and mobile device
4.	Enable wake on LAN in PC and configure WOL on mobile device
5.	Install Active Directory Domain Services
6.	Configure Active Directory Domain Services and create local Root Domain
7.	Proceed to mk-optiplex7090 step 1-4
8.	Verify that mk-optiplex7090 has been added in Active Directory Computers
9.	Create new user account (mkyuson) and proceed to mk-optiplex7090 step 5
10.	Create SMB share and proceed to mk-optiplex7090 step 7

mk-optiplex7090 steps:
1.	Install Windows 11 Pro
2.	Configure Windows 11 Pro (change PC-name, set MKtech-ADDC IP Address as preferred DNS, set 8.8.8.8 as alternative DNS and restart the PC)
3.	Test if connection to the Root Domain is successful by using nslookup and ping command.
4.	Join mk-optiplex7090 to the domain and proceed to MKtech-ADDC step 8
5.	Login as new user account (mkyuson)
6.	Change user account password (mkyuson) and go back to MKtech-ADDC step 10
7.	Verify if SMB share is accessible to the PC

---

Details:\
PC-Name\
MKtech-ADDC

Administrator\
Password1

Root Domain\
MKtech.local

Directory Services Restore Mode (DSRM)\
Password1

Mark Yuson(AD account)\
mkyuson\
Password1

PC-Name\
mk-optiplex7090

MicroW11 (local account)\
Password1

Note: All passwords are incorrect and for documentation purpose only.

References:
WOL: https://www.dell.com/support/kbdoc/en-ph/000175283/how-to-setup-wake-on-lan-wol-on-your-dell-system
