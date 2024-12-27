<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How to Setup a Domain Controller for Active Directory (On An Azure VM)](https://www.youtube.com/watch?v=CRItvaqJjjY&ab_channel=Z)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022

<h2>High-Level Deployment and Configuration Steps</h2>

- Setup Azure VNet & Windows Server VM
- Follow "Add Roles and Features" Wizard
- Add "Active Directory Domain Services" Role
- Promote Server to Domain Controller & Restart
- "Add a New Forest" and Create Domain Name and DSRM Password
- Restart Server and Log in to Domain with Domain Name Context

<h2>Deployment and Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/R20lWZa.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Create virtual network and a Windows Server VM inside of Azure. Be sure the VM is in the same region and on the created virtual network.
</p>
<br />

<p>
<img src="https://i.imgur.com/JONEZKI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Follow along with the wizard, being sure to add the "Active Directory Domain Services" Role.
</p>
<br />

<p>
<img src="https://i.imgur.com/vxF1idM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Promote server to domain controller.
</p>
<br />

<p>
<img src="https://i.imgur.com/zOxVkAq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Add a "New Forest" and create a dommain name. Click next and create DSRM password.
</p>
<br />

<p>
<img src="https://i.imgur.com/C6EtcBw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Restart and log back into domain with proper context (domainname\username). Congrats! Active Directory is deployed on your domain controller!
</p>
<br />
