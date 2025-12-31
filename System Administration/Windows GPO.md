# Windows GPO
Tags: #windows , #gpo
Author: Shahid Sharif
Initial Release: 21Aug2022
Last Update:  21Aug2022
Reference: 



1.  Demo Configuration Videos and Guides: [https://www.rtsnetworking.com/demo](https://www.rtsnetworking.com/demo)
2.  Access Microsoft Self Paced Labs: [https://www.microsoft.com/handsonlabs](https://www.microsoft.com/handsonlabs)
3.  Group Policy can be used to manage:
	1.  Network Settings
	2.  Desktop Settings
	3.  Security Policies
	4.  Folder redirection
	5.  Software deployment
	6.  Application restrictions
	7.  Logon scripts
	8.  Audit Policies
4. Group Policy Processing Order
	1.  Local- applies to local computer gpedit.msc or MMC snap-in
	2.  Site-Applies to an AD site.  A site represents a physical location
	3.  Domain-Applies to the AD domain
	4.  Organizational Unit(OU)-applies to an OU
5. Group Policy
	1.  Block Inheritance
	2.  Enforced
	3.  Security Filtering
	4.  WMI Filtering: Uses scripts written in WQL
6. WMI:  Windows Management Instrumentation
7.  Administrative Templates
	1.  Allows management over settings that cannot be managed by default, such as Google Chrome
	2.  .ADM: Legacy. Windows XP and server 2003
	3.  .ADMX: XML files, extensible, 3rd party, language neutral
	4.  ADML: Language file
8. Central Store
	6.  Default location for administrative templates: c:\windows\PolicyDefinitions
	7.  Central store must be manually created
	8.  c:\windows\SYSVOL\sysvol\<DomainName>\policies\policydefinitions
	9.  Replicates to all domain controllers in the domain
	10.  Automatically detected when editing policies
9.  Security Settings that can be defined in a GPO
	1.  Account policies
	2.  Windows firewall configuration
	3.  User rights assignments
	4.  Audit policy
	5.  Restricted Groups
10. Group Policy Scripts
	1. Run logon scripts synchronously
	2.  Run startup scripts synchronously
	3.  Maximum wait time for Group Policy scripts
	4.  If windows PowerShell is used to write scripts, the scripts require signing or the script execution policy will have to e reduced, which decreases security.
12. Group Policy Software Deployment
	1. Advantages
		1.  Defined within a GPO
		2.  Deploy to computers or Users
		3.  Deploy by site, domain, OR
		4.  Additional tools not required
	2. Disadvantages
		1. Lack of scheduling
		2.  Bandwidth saturation
		3.  Limited reporting
		4.  Only deploy .MSI packages
		5.  May require security filtering
13. GPO Preferences
	1. Preference are only available in active directory level policies
	2.  Applied as the site, domain and OU Level
	3.  Can be made optional
	4.  Support for item-level targeting
15. Managing Group Policy Backups
	1. GPO Backup
	2.  BPO restore:
	3.  GPO Import
	4.  GPO Copy
17. Troubleshooting GPO Issues
	1.  Gpresult: gpresult /h <reportname.html>
	2.  Group Policy results
	3.  Group Policy Modeling
	4.  DCGPOFIX: To reset to factory default domain and default domain controller policy