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

- Create Vm and resources in Azure
- Ensure Connectivity between client and Domain Controller
- Install Active Directory
- Create admin and normal user account in Active Directory

<h2>Deployment and Configuration Steps</h2>

<p>
<img src="https://imgur.com/3aIF852.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In this step I created the Virtual machine and subnet,and the domain controller Vm(using windows server) named DC-1. I also created the client computer VM(Window 10)"Client-1."
</p>
<br />

<p>
<img src="https://imgur.com/dV9dXvZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Here I set the Domain Controllers NIC IP address to static so it does not change and so that the client computer can actually join the Domain and it will use the Domain Controller as it's DNS server.I manually set the client computer to do this so that the DNS server did not create a random IP address for the client computer. 
</p>
<br />

<p>
<img src="https://imgur.com/utNILdi.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In this step I installed active directory domain services on the Domain Controller server.
</p>
<br />
