The script needs PowerShell 4 installed, please see the below link to install:

https://social.technet.microsoft.com/wiki/contents/articles/21016.how-to-install-windows-powershell-4-0.aspx

When running the checks powershell script it uses some external files, please make sure to run from the bootstrap wavenetmaint.ps1 file to make sure you're running the correct verions and have all the files.

Known issues
============
Last login check for users only shows from server script is being run from. Fix being investigated to query all DCs.

Change History
==============

v0.9.5
Check and allow RDP inbound though firewall
disable MWService user account
Removed old RMM GPO

v0.9.4
install AD Bitlocker tools
added output of AD Connect version
added block Win11 GPO import


v0.9.3
added GPO for DisableFastStartup

v0.9.2
added GPO to store Bitlocker recovery in AD

v0.9.1
delete SSL Cipher GPO
add in hardend netlogon and sysvol unc paths
fix for not deleting zip files
make windows update cleanup optional

v0.9
Cleanup c:\sagebackups
no longer removes old zip files from maint output
now checks for pyranet and wavenet rmm gpo and if imports its as wavenet

v0.8 
Add option for WinSxS cleanup

v0.7

Removal of StorageCraft ShadowControl
Defrag of Windows Search index
Enable inbound PING check

v0.6.1

Fixed issue with time service reset for PDC Emulater
Added power plan change prompt

v0.6

Added Windows Defender removal
Added Power Plan output

v0.5

Added Hyper-V checks

v0.4
Added RMM GPO check and import
added check for speculation control files

v0.3.3
Added in PowerShell 4 requirement check

v0.3.2
Fixed some typos

v0.3.1
Added check and delete for *.mdmp files in c:\ProgramData\AVAST

v0.3
Added Pulseway check and removal

v0.2.10
Added AD DFSR check
Date stamp added to output files
Creates a zip file of output
Added colour to some output in powershell window

v0.2.9
Added users last logon date to users.csv

v0.2.8
Added Subnet list dump

v0.2.7
Added Server list dump

v0.2.6
Changed user.txt to use UPN for usernames

v0.2.5
Added SpeculationControl for meltdown and spectre

v0.2.4
Added requires run as admin check

v0.2.3
Hidden some error output

