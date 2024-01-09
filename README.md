<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the installation of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)



<h2>Installation Steps</h2>

<p> Step 1: <b> Create Cirtual Machine in Azure </b> </p>

<img src="https://i.imgur.com/gfFwjXl.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
</p>
<p>
1. Create a new resource group </p>
2. Create a Windows 10 Virtual Machine (VM) with 4 virtual CPUs as the size </p>
3. Remember to take notes of the username and password you create </p>
4. Under the network tab, allow it to create a new virtual network (vnet) </p>
5. Click review and create! </p>
</p>
<br />

<p>
<img src="https://i.imgur.com/bGPk2a4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Pre-installation, I enabled IIS in Windows with CGI and common HTTP features. Then I installed PHP Manager for IIS and Rewrite Module. I created the directory C:\PHP, as well as MySql. Finished with Install of osTicket.
</p>
<br />

<p>
<img src="https://i.imgur.com/EXr7iBl.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Loaded osTicket and verified a successful login.
</p>
<br />
