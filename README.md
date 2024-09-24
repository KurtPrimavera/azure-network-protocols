<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>DNS Management Strategies and Effective Permissions for Network File Sharing</h1>
In this tutorial, we explore the fundamentals of DNS management and experiment with network file shares. Participants will learn how to configure and manage DNS settings to ensure efficient name resolution within their networks. Additionally, we will delve into the setup of network file shares, examining how to create shared resources and assign permissions to users and groups. By engaging in hands-on experiments, users will gain practical experience in both DNS management and the effective administration of network file shares, enhancing their skills for real-world applications. <br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure – Virtual Machines and Compute resources
- Remote Desktop Protocol (RDP) – Remote access to virtual machines
- Command-Line Tools – Including PowerShell and CMD for system management
- Network Protocols – SSH, RDP, DNS, HTTP/S, ICMP for communication and connectivity
- Wireshark – Used for protocol analysis and network traffic monitoring
- DNS Management – Configuration and troubleshooting of DNS settings
- Server Manager – For managing server roles and features
- Active Directory – User and group management within the domain
- Security Groups – Permissions and access control for users and resources
- PowerShell ISE – Scripting and automation tasks for administrative purposes
- File Explorer – Managing network file shares and permissions

<h2>Operating Systems Used </h2>
- Windows 10 (21H2) – Operating system for virtual machine deployment and testing environments
- Ubuntu Server 20.04 – Linux-based server OS for network services and application management


<h2>High-Level Steps</h2>
1.	Created and Deleted A Records – Managed DNS A records for IP address mapping.
	2.	Created CNAME Records – Established canonical names for domain aliasing.
	3.	Edited Root Hints – Modified root hints for improved DNS resolution.
	4.	Checked Local DNS Cache – Verified and cleared the local DNS cache.
	5.	Created Fully Qualified Domain Name (FQDN) – Defined FQDN for complete domain identification.
	6.	Implemented Command-Line Tools – Utilized command-line utilities for DNS management and troubleshooting.
	7.	Configured File Shares – Set up and managed network file shares for user access.
	8.	Located Domain Controller in File Explorer – Accessed and verified the domain controller through the file explorer interface.
<h2>Actions and Observations</h2>

<p>
<img src="https://github.com/user-attachments/assets/3f4d9e7f-02d1-479c-9481-3428e23a4766"/>
</p>
<p>
	•	Set Up A Records in PowerShell ISE – Utilized PowerShell Integrated Scripting Environment (ISE) to create and manage A records, which map fully qualified domain names (FQDN) to specific IP addresses. This process ensures that when users enter a domain name in their browser, it resolves to the correct server hosting the website or service.
	•	Configured CNAME Records – Established Canonical Name (CNAME) records to create aliases for existing domain names. This allows multiple domain names to point to the same IP address without needing separate A records. For example, if “www.example.com” is a CNAME for “example.com,” both will direct users to the same website.
	•	Edited Root Hints – Modified the root hints in the DNS server settings to improve its ability to communicate with other DNS servers across the internet. Root hints are essential for DNS resolution, as they help the server locate authoritative DNS servers when resolving domain names that are not cached locally.
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/835a09f8-6832-4931-a92b-950be7465dc0"/>
</p>
<p>
	•	Checked Local DNS Cache on the Domain Controller – Verified the local DNS cache to ensure that it correctly reflected the current DNS records. This step is crucial for troubleshooting DNS resolution issues within the domain.
	•	Utilized Nslookup to Search DNS Records – Employed the nslookup command to query DNS records stored in the domain controller. This tool helps confirm that the domain controller is returning the correct DNS information for various domain queries.
	•	Executed ipconfig /displaydns to Resolve DNS Cache – Ran the command ipconfig /displaydns to view the contents of the local DNS cache, which includes previously resolved domain names and their corresponding IP addresses. This helped identify any outdated entries that may need to be refreshed.
	•	Identified Old IP Addresses in DNS Cache – Noted that the DNS cache contained an old IP address, which could cause connectivity issues if clients were attempting to reach a resource that had since changed.
	•	Executed ipconfig /flushdns to Clear Old DNS Entries – Cleared the DNS cache by using the command ipconfig /flushdns, removing outdated records and ensuring that new DNS queries would be resolved accurately.
	•	Utilized Root Hints for External DNS Resolution – Configured root hints to enable the domain controller to query other DNS servers when it cannot resolve a domain name locally. This feature is essential for effective DNS resolution in environments where records may be hosted externally.
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/59677c07-509f-43e2-b4d6-587ed26ec406"/>
</p>
<p>
	•	Configured Properties for Domain Users – Adjusted various attributes and settings for domain users within Active Directory, including usernames, passwords, contact information, and group memberships. This configuration ensures that users have the correct access levels and security settings in line with organizational policies and compliance requirements.
	•	Located Domain Controller on the Network – Successfully identified the domain controller’s IP address and hostname within the network infrastructure. This step involved verifying network connectivity and confirming that the domain controller is operational, which is crucial for user authentication, policy enforcement, and resource management.
	•	Edited Security Groups for File Sharing – Modified the permissions of specific security groups to effectively manage file sharing across the network. This included setting access levels such as read, write, or deny for various files and directories, ensuring that sensitive data is protected while allowing authorized users to access necessary resources.
	•	Changed Users’ Roles – Updated the roles and responsibilities of users in Active Directory to align with changes in their job functions or organizational structure. This process involved reassigning users to appropriate groups and updating their permissions, ensuring that they have the necessary access to perform their tasks while adhering to the principle of least privilege.
</p>
<br />
