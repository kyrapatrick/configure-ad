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

- Step 1
- Step 2
- Step 3
- Step 4

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
