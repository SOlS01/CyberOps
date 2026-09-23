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

 
 

# Module 5 >> 

Route tracing 

Common network protocol for network communication is HTTP/TCP/IP.   

TCP/IP protocol includes many protocols for example: 

Application > name system it uses DNS, file transfer it uses FTP/SFTP/TFTP, for web service it uses HTTP/HTTPS (set of rules for exchanging text, sounds, ...), for host config it uses DHCPv4 and 6/SLAAC (a method that allows a device to have IPv6 address without using DHCPv6 server), for email uses SMTP (simple mail transfer protocol)/POP3/IMAP. 

Transport Layer >> TCP (connection oriented) and UDP (connectionless) 

Internet Layer >> internet protocol it uses IPv4 and 6 and NAT, for messaging it uses ICMPv4 and 6,  

Network access layer >> address resolution it uses the ARP, for the data link protocol it uses the Ethernet. 

 

Message timing >>  

Flow control: it defines how much information can be sent and the speed at which it can be delivered. 

Response timeout:   

Access method: it determines when someone can send a message. 

Unicast is a one-to-one delivery option, multicast is when a host needs to send messages using a one-to-many delivery options, broadcast if all the hosts need to receive the message at the same time. 

 

The benefit of using layered model >> OSI open system interconnection, TCP/IP 

Each layer can have its own protocol  

Preventing technology and capability in one layer from affecting other layers  

Providing a common language to describe networking 

 

# Description of OSI model Layers: 

Application: the application layer contains protocols used for process to process communication 

Presentation: it provides for common representation of the data transferred between application layer services. 

Session: it provides services for presentation layer to organise its dialogue and to manage data exchange. 

Transport: it defines services to segment, transfer and reassemble the data for individual communications between the end devices 

Network: it provides services to exchange the individual pieces of data over the network between identified end devices. 

Data link: it describes methods for exchanging data frames between devices over a common media 

Physical layer: describe the mechanical, electrical, active or de-activate physical connections 

# TCP/IP model description: 

Application: represent data to the user and encoding and dialog control 

Transport: supports communication between various devices across diverse network 

Internet: determine the best path through the network 

Network access: it controls the hardware devices and media that make up the network 

Message segmenting has its own benefit which is increase speed and increase efficiency for example when one of the segments failed because of the network congestion only that one needs to be send again. 

Sequencing is important because the receiver needs to be able to reassemble the data again, so sequence number is needed. 

 

Protocol Data Unit (PDU) >> it happens during encapsulation where each layer adds its own and passes it down to other layer. 

Data-data-data-segment-packet-frame-bits 

 

# For network communication we need 3 addresses: 

Transport layer uses protocol address (port number) to identify network applications that should handle client and server data. 

Network layer it specifies addresses that identify the clients and servers which attached to the clients and servers,  

Data link it specifies the devices on the local LAN that should handle data frame. 

Encapsulation example >> data then TCP segments then IP packets and all in an ethernet frame will be sent to the web client it is called the protocol stack. 

Decapsulation is encapsulation backward, (decoding ) 



# Module 6 >> 

Ethernet: it operates in data link layer and physical layer, defined in the IEEE 802.2 and 802.3, specifies that a network implement the CSMA/CD access control method.the min ethernet frame size is 64 bytes and max is 1518. Preamble is not included in the size. If the transmitted frame is not in the range size, then it will be dropped by the receiving device. 

# Field of ethernet frame:  

Preamble: start of the frame, used for synchronisation between the sending and receiving device., it is used to get the attention of the receivers and tell them to get ready to receive a new frame. 8byte 

Destination MAC address: identifier for the intended recipient, used by Layer2 to assist devices in determining if a frame is addressed to them. 6byte 

Source MAC address: it identifies the originating NIC or interface of the frame; a source MAC address can only be a unicast address. 6byte 

Type/length: it identifies the upper layer protocol encapsulation in the ethernet frame. 2 bytes 

Data field: it contains the encapsulated data from a higher layer, all must be 64bytes if not additional bits called a pad are used to increase the size of the frame to the minimum size. 

Frame check sequence: it is used to detect errors in a frame; it is used the cyclic redundancy check. 

MAC address can be represented with dashes 00-60-2F-3A-07-BC, colons, periods 0060.2F3A.07BC 

Data link layer is responsible for raking an IP packet and preparing it for transmission over the communication medium. 

 

# Network Layer >>  

IPv4, IPv6, open shortest path first OSPF, internet control message protocol ICMP 

This layer encapsulates the protocol data unit from the transport layer into a packet. 

IP encapsulates the transport layer segments by adding an IP header which is used to deliver the packet to the destination host. This IP headers examined by layer 3 devices like router and layer 3 switches, IP remains the same after leaving the source host until it arrives to the destination except NAT for IPv4 because it is used a public IP address for private for extra security. 

Connectionless means there is no connection with the destination before sending data. Best effort means there is no guarantee in packet delivery. Media independent means operation is independent of the medium like fiber-optic or wireless carrying the data. 

Fragmentation it is when a router must split up an IPv4 packet when forwarding it from one medium to another one because of the maximum transmission unit, fragmentation causes latency. IPv6 cannot be fragmented by the router. 

The IPv4 packet header is used to ensure that this packet is delivered to its next stop on the way to its destination end device, the header checksum used to detect corruption in the IPv4 header. 

 

Subnet mask is used to identify the network/host portion of the IPv4 address. 1 for the network portion and 0 for the host portion. 

The more broadcast traffic is good but in other hand it will slow down the internet. 

Reserved private IPv4 address >>  

10.0.0.0/8 - 172.16.0.0/12 - 192.168.0.0/16 NAT network address translation is used to translate between private IPv4 and public IPv4 addresses  

Network layer direct packets between hosts > hosts can send packet to:  

To ensure that their packets are dedicated to the correct network destination they must keep their own local routing table that contains a route to the loopback interface, a local network route, and a remote default route. 

Itself > ping itself which is a loopback interface. 

Local host > destination host in local network 

Remote host > destination host on the remote network 

 Default Gateway is the network device which can route traffic to other networks. 

Host Routing Table >> to display we need route print and netstat –r commands 

 

IPv6 addresses are 128 bits, and its prefix length can till 128, every 4 bits represent by a single hex which is 16 binary digits,  

Rule one >> omit the zeros from the left-hand side in each hextet to reduce notation. 4 zeros will be one 0 

Rule two >> to reduce notation a double colon can replace any single or same near each other strings consist of all zeros. (after rule 2 delete same strings in row when they placed near each other if they are 3 or 4 separates then instead leave 2 colon) 

Ex: 2001:0db8:0000:0000:ab00:0000:0000:0000 >> 2001:db8:0:0:ab00:: 

Pinging 127.0.0.1 is the local loopback address on any TCP/IP network device, to verify the protocol stack on a particular device. 

ANDing allow us to identify the network address of the destination network. 


 

# Module 7 >> connectivity verification 

ICMP can help us understand both normal and abnormal network behaviour, they create special packets that test the network.  

Host confirmation: to determine if a host is operational or not 

# Destination or service unreachable: codes for it are > 0 net/ 1 host/ 2 protocol/ 3 port 

Time exceeded 

Route redirection 

 

ICMPv6 includes four new protocols as part of the neighbour discovery protocol >> message between IPv6 router and device, router solicitation and advertisement  

Message between IPv6 devices, neighbour solicitation (when the devices know the IP but not the MAC it is the same as ARP) and advertisement (it is the response with the ethernet MAC address of the device) 

We can ping each device and the router to make sure about their connectivity, if we couldn’t ping a router its maybe because the default gateway configured wrong or because of security purposes it prevents the response. 

Traceroute is a utility that generates a list of hops that were successfully reached along the path. An asterisk * is used to indicate a lost or unreplied packet. TTL or time to live will continue to increase until it reaches the destination but each time it will get to a hob will send a time exceeded message back and start over to find new hob until getting to the destination. 

ICMPv6 uses DAD to make sure that a unique IPv6 is configured on the interface. 

# ICMP packet format >>  

It is encapsulated directly into IP packets; it is like the transport layer. Common codes are: 0 echo reply/ 3 destination unreachable/ 5 redirect/ 8 echo request/ 11 time exceeded
