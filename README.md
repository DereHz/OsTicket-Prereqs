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

  
<img width="1078" alt="Screen Shot 2024-05-19 at 9 11 36 AM" src="https://github.com/DereHz/osTicket-prereqs/assets/169094076/472a4d2f-9633-4839-bff1-92fe174f459e">

Step 2. Create a Windows 10 pro Virtual Machine (VM) with 2-4 Virtual CPUs
  -  Name: VM-osTicket
  - Username: labuser (or what ever you decide to choose for a username)
  - Password: osTicketPassword1!(example)
  - When creating the VM, Create a new Virtual Network (Vnet) 
  - Click Review+Create

  
<img width="1849" alt="Screen Shot 2024-05-19 at 9 16 44 AM" src="https://github.com/DereHz/osTicket-prereqs/assets/169094076/dc073a69-65c0-41f4-87ab-fdfb053814b6">

Step 3. Open Microsoft Remote Desktop (If on Mac Desktop)
  - Click Add PC and enter your VMs public IP (Wait until the VM finishes deploying) 
  - Enter the username and password you put in for your VM


<img width="1214" alt="Screen Shot 2024-05-19 at 9 36 44 AM" src="https://github.com/DereHz/osTicket-prereqs/assets/169094076/ca4884b9-8dfb-4198-a555-f2368427475d">

Step 4: Install/Enable IIS in Windows with CGI and Common HTTP features 
- right click on the "start" icon, Click run, and enter "control"
- Click on "programs" and then "turn windows features on or off"
- clikc on internet information services -> World Wide Web Services -> Application Development Features ->
[X] CGI
[X] Common HTTP Features
- Internet Information Services -> Web Management Tools -> IIS Management Console
	[X] IIS Management Console
- Click Ok

<img width="1532" alt="Screen Shot 2024-05-19 at 10 11 10 AM" src="https://github.com/DereHz/osTicket-prereqs/assets/169094076/f752a179-4c8d-4696-9977-e19c824f6054">
  
Step 5. Open the Installation files page here:
(https://drive.google.com/drive/u/1/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6) 
- Download and isntall PHP Manager for IIS
- Download and install Rewrite Module
- Download and install PHP 7.3.8
- Download and install VC_redist.x86.exe.
- Download and install MySQL 5.5.62
  When MySQL downloads: Typical setup -> Launch Configuration Wizard(after install) -> Password1
  
Note: if you dont see anything happen immediately after clicking download, give it a few seconds. 


<img width="1332" alt="Screen Shot 2024-05-19 at 10 04 33 AM" src="https://github.com/DereHz/osTicket-prereqs/assets/169094076/8a72fa53-8fbf-4840-bdc3-1ed62d68511f">

When PHP 7.3.8 is finished downloading, Create a folder "PHP" on Windows (C:). right click the PHP 7.3.8 file -> extract all -> browse -> This PC -> Windows (C:) -> PHP -> Select Folder -> Extract


