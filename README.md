# CyberOps from Cisco 

# Module 1 >> The Danger 

Threat actors: 

Amateur = script kiddies, uses existing tools. 

Hacktivists = protesters against organisation and government, DDoS. 

Financial gain = also known as organised crime group they are cybercriminals who hack to generate cash. 

PII = personal identifiable information, distinguish identities of individuals 

PHI = personal health information 

PSI = personal security information 

Stuxnet is an example of the national security concern 

Malware attack >> it is to disrupt computer operation + gather sensitive information + gain access to private computer system for example searching and obtaining trade secrets. 

A worm has got the primary objective of spreading across the network. 

 

# Module 2 >> Fighter against cybercriminals 

Cyberwarfare is an internet-based conflict that involve the penetration of the network and computer system of the other nation. The purpose of it is to gain advantage over adversaries over both nations and companies. 

Elements of SOC: Process, Technology, People 

SOC can provide managing comprehensive threat solutions + monitoring network security threats 

4 tiers in SOC >>  

Tier 1 = alert analysts, monitoring, verifying true incidents, opening tickets 

Tier 2 = incident response, responsible for deep investigation, advise remediation and action. 

Tier 3 = threat hunter, expert level skill in network, malware reverse engineering, threat intelligence. 

SOC manager  

Technologies in SOC: 

SIEM (system information and event management) it acctually combines data from multiple sources to help SOC, it is used to collect, filter, detect and classifying the threat, it can by collecting data and filter them help SOC against security threats + SOAR (security orchestration automation and response) it is like the SIEM but goes further it works based on a playbook that developed by the security team. 

SOC monitoring system includes security monitoring, security control, log management, vulnerability assessments, vulnerability tracking, threat intelligence, event collection and analysis. 

SOC metrics:  

Dwell time > the length of access time before being detected and stopped access. 

Mean time to detect MTTD > identify the valid security incident 

Mean time to respond MTTR > stop and remediate an incident 

Mean time to contain MTTC > time require to stop the incident from causing further damage 

Time to control > time to stop the spread of the malware in the network. 

 

# Module 3 >> Windows Operating System 

Dir = Lists directories 

Cd directory = Changing to the desire directory 

Cd / = Go to the root directory 

Cd ..  = Go above the current directory 

Mkdir = Making a directory 

Ren = To rename a file 

 

Operating system vulnerability >>  

A good security policy must be configured and followed because it can prevent attacks. 

Firewall is to limit communication with devices on the network. 

Kernel is the core of the operating system and hardware abstraction layer is a software that handles all the communication between the hardware and the kernel, kernel is communicate with the hardware but it’s not completely independent of the HAL. 

Windows File System >> how information is organized on storage media. 

exFAT > number of partition limitation, partition size, not used for SSD and HD, FAT32 and FAT16 

HFS+ > windows are only able to read data from it, used on MAC OS. 

EXT (extended file system) > used with Linux based computers, windows can read data with special software. 

NTFS > commonly used and all Windows and Linux version support it but MAC OS can only read data from it. (support recovery features, very large files and reliable, track the time stamps, support file system encryption) 

# Windows Boot Process >>  

Compute firmware: BIOS and UEFI (it will increase the security because goes straight to protect mode,) 

The MBR master boot record is responsible for locating and loading the operating system, it is a traditional partition scheme for hard drive. 

To configure windows processes we search for the Task Manager. 

Virtual address support for 32-bit windows is 4GB and for 64 is 8T. 

Windows Registry > information about hardware, application, users, system settings, the registry also has a unique section for personal user configuration. (a hierarchical database of all system and user information) 

- HKEY_Current_user: currently logged in user 

- HKEY_Users: information about all the user account on the host. 

- HKEY_classes_root:  

- HKEY_local_machine: hold system information 

- HKEY_current_config: information about the current hardware profile. 

To modify the registry, we can use the tool called regedit.exe 

To manage the local users and groups we can use lusrmgr.msc control panel. 

PowerShell is an integrated program within Windows >  

- Cmdlets: perform an action and return an output to the next command that will be executed 

- PowerShell scripts: .ps1 extension 

- PowerShell function: codes that can be referenced in a script 

 

# Common net command >  

Net account = Set password + login requirements for users 

Net session = Lists or disconnects session 

Net share = Create, remove, manage shared resources 

Net start/stop = Start/stop a network 

Net use = Connect/disconnect and display information about a shared network resource 

Net view = List of the computers and networks on the network 

 

# Task Manager >  

Processes = Running process and programs, display CPU,  

Performance = Overview of the CPU and memory and disk,  

App history 

Startup = Applications and services that start when the computer boot 

Users = Logged on users on the computer, resources they used, administration can disconnect a user 

Details 

Services = Loaded services,  

 

# Nslookup (to find the address of a website/ server from a URL, used to test the DNS if it is function correctly/ ipconfig only display previously resolved DNS entries.) (also ping to check if DNS name resolution is working properly on a windows PC) and netstat (to see details of active network connections with their status and TCP protocols, it looks for inbound or outbound connection that are not authorised) 

SMB server message block protocol is used to share network resources it is mostly used to access files on remote hosts. 

An administrative share can be identified with $ that comes after the share-name. 

To find the process ID we can go to the Task Manager and right click on that. 

Event viewer logs valuable information like history of application and security to help identify a problem and maintains system logs. 

Windows defender firewall denies traffic to a computer or network segments. And Windows defender has a built-in virus and spyware protection. 

On resource monitor we can see the CPU, DISK, network. 

Windows system that are not part of an active directory domain can use the windows local security policy to enforce security setting on each stand-alone system. 

# Windows boot sequence >>  

1. The windows boot loader winload.exe 

2. Ntoskrnl.ece and hal.dll 

3. Winload.exeis 

4. Ntoskrnl.exe and execute 

5. Winlogon.exe and execute the logon process 

 

Module 4 >> Linux Operating System 

Linux distributions are free to use but support is at a charge. Perfect for SOC as the OS can be tailored to become the perfect security analysis platform. 

SOC tools >>  

- Network packet capture software: Wireshark, to observe and understand every detail of a network transaction 

- Malware analysis 

- IDS intrusion detection system: real time traffic monitoring and inspection searching based on a predefined rule. 

- Firewall  

- Log managers 

- SIEM system information and event manager, real time analysis of alert and log entries  

- Ticketing system 

Kali Linux is the distribution for pen testing. 

mv = Move or rename 

chmod = Change file permission 

chown = Change ownership 

dd = Copy data from an input to an output 

pwd = Display the name of current directory 

ps = List current running processes 

sudo = Run command as a super user, super user privilege 

grep = search 

Apt = Used to install 

cat = List the content of a file 

Man  = Display the documentation (syntax and parameters) for a specific command 

mkdir = Make directories 

cd = Change current directory 

ls = Display the files inside a directory 

 

In Linux everything is a file, Nano is a command line text editor which is used for system configuration and maintenance in Linux.  

Control + O= save / control +w= search menu / control + G= help 

# Well known ports >>  

20/21, 69 = FTP, TFTP 

22 = SSH 

23 = TELNET 

25 = SMTP simple mail transfer protocol 

53 = DNS 

67/68 = DHCP 

80/443 = HTTP/HTTPS 

 

Hardening a device >> securing the device with methods and protect its administrative access. Minimise installed packages, physical security, disable unused services, diable a root account login for SSH and use SSH, update regularly, strong password, periodic password, no old password. 

Daemons is a background process that runs without the need for user interaction. 

# Linux log files >>  

/var/log/message = Information and non-critical Debian-based 

Auth.log = User authentication related things Debian and Ubuntu 

secure = Tracks sudo login/SSH login and error logins RedHat 

Boot.log 

dmesg 

Lern.log 

cron 

Mysql.log = All debug, failure, and success go there. RedHat CentOS and Fedora use with sqld and Debian and Ubuntu use sql in the name of the file 

 

# File system type in Linux >>  

ext2 

ext3 = Max size 32TB, designed to improve ext2 

ext4 = Improved the ext3 and increase support file size 

NFS network file system 

HFS+ = File system used by Apple,  

APFS apple file system = Update file system used by apple provide strong encryption and it’s for flash and solid-state drive. 

MBR master boot system = First sector of partitioned computer 

 

Roles and permission >>  

We got users/ group/ others in a directory permission (read R, write W, execute X) . - or / indicate the directory. The only user that can override file permission on Linux is the root user. 

Rootkit >> a type of malware which designed to increase an unauthorised user’s privilege and grant the access it will also be used to secure a backdoor. 

To combine two commands, we can use the pipe | it will feed the output of one command into the input of another. 

Ps command from an admin is to list the process currently running in the system. 

 
