# osTicket-prereqs
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- PHP Manager For IIS
- Rewrite_amd64_en-US.msi
- php-7.3.8-nts-Win32-VC15-x86.zip
- VC_redist.x86.exe
- My SQL 5.5.62
- OS Ticket v1.15.8
- HeidiSQL

<h2>Installation Steps</h2>

<img width="1767" alt="Screen Shot 2024-05-19 at 9 08 59 AM" src="https://github.com/DereHz/osTicket-prereqs/assets/169094076/35d881bb-b0d7-4969-a021-d7b583ec2343">

Step 1. Create a Resource Group in Azure 
  
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Step 2. Create a Windows 10 pro Virtual Machine (VM) with 2-4 Virtual CPUs
  -  Name: VM-osTicket
  - Username: labuser (or what ever you decide to choose for a username)
  - Password: osTicketPassword1!(example)
  - When creating the VM, Create a new Virtual Network (Vnet) 
  - Click Review+Create
  
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Step 3. Open Microsoft Remote Desktop (If on Mac Desktop)
  - Click Add PC and enter your VMs public IP (Wait until the VM finishes deploying) 
  - Enter the username and password you put in for your VM

</p>
<br />
