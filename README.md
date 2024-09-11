<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>DNS Management and Network File Shares and Permissions</h1>
In this tutorial, we observe DNS management and experiment with Network File Shares <br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop Protocol
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
- Implemented cmd line tools
- Configured file shares
- Located domain controller in file explorer

<h2>Actions and Observations</h2>

<p>
<img src="https://github.com/user-attachments/assets/3f4d9e7f-02d1-479c-9481-3428e23a4766"/>
</p>
<p>
Set up A records in Powershell ISE. CNAME maps the IP address to another name. Root hints communicate with other DNS servers. 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/835a09f8-6832-4931-a92b-950be7465dc0"/>
</p>
<p>
Checked local DNS cache if in the domain controller. Nslookup searched DNS records in the domain controller. ipconfig /displaydns resolved the DNS cache. The old IP address was the DNS cache. ipconfig /flushdns deleted old dns. Root hints use other servers to solve DNS if it can't find it locally. 
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/59677c07-509f-43e2-b4d6-587ed26ec406"/>
</p>
<p>
Configured properties for domain users. Located domain controller on the network. Edited security groups for file sharing such as read, write, or deny to files. Changed users' roles.  
</p>
<br />
