<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Create 2 virtual machines using Azure:"DC-1" domain controller (server); "Client-1" (Windows 10)
- Install Active Directory on DC-1 and join Client-1 to the domain 
- Create user accounts (Domain users) in Active Directory 
- Create folders in Active Directory and explore file shares on the network and permissions
- Explore configuring DNS records

<h2>Deployment and Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/pFXNRLa.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Login to virtual machine DC-1 and install Active Directory Domain Services by selecting "Add roles and features". Installation completed by promoting server to Domain Controller. 
</p>
<br />

<p>
<img src="https://i.imgur.com/DxJz8p0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Organizational Groups "EMPLOYEES" AND "ADMINS" are created and Client-1 virtual machine is joined to the domain.
</p>
<br 

<p>
<img src="https://i.imgur.com/RrINqKn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Domain users created and allowed access to remote desktop.
</p>
<br />
<p>
<img src="https://i.imgur.com/uU03Q5z.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Network Access shows Domain users have "Read" access.
</p>
<br />
<p>
<img src="https://i.imgur.com/TfE6ciQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
A-Record "mainframe" created with IP address: 10.0.0.4.
<br />
<p>
<img src="https://i.imgur.com/cT6tsZn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
DNS display showing "mainframe" A-Record with IP address 10.0.0.4
<br />
<p>
<img src="https://i.imgur.com/QnWTUF6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
A-Record "mainframe" showing new IP adress 8.8.8.8
<br /> 
<p>
<img src="https://i.imgur.com/FsUDYVv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
DNS display "mainframe" A-Record showing new IP address 8.8.8.8
<br />   
