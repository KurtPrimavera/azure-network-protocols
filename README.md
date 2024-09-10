<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>DNS Management and Network File Shares and Permissions</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)
- DNS
- Server Manager
- Active Directory
- Security Groups
- Powershell ISE
- File Explorer

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

- Created and deleted A records
- Created CNAME
- Edited Root Hints
- Checked local DNS cache
- Created FQDN
- Implemened cmd line tools
- Configured file shares
- Located domain controller in file explorer

<h2>Actions and Observations</h2>

<p>
<img src="https://github.com/user-attachments/assets/3f4d9e7f-02d1-479c-9481-3428e23a4766"/>
</p>
<p>
Set up A records in Powershell ISE. CNAME maps ip address to another name. Root hints communicate with other DNS servers. 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/835a09f8-6832-4931-a92b-950be7465dc0"/>
</p>
<p>
Checked local dns cache if in the domain controller. Nslookup searches Dns records in domain controller. ipconfig /displaydns resolved Dns cache. The old ipaddrress was the Dns cache. ipconfig /flushdns deleted old dns. Root hints uses other servers to solve dns if it can't find it locally. 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/59677c07-509f-43e2-b4d6-587ed26ec406"/>
</p>
<p>
Configured properties for domain users. Located domain controller on the network. Edited security groups for file sharing such as read, write, or deny to files. Changed users roles.  
</p>
<br />
