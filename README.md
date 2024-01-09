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

<p> Step 2: <b> Installion </b> </p>
<img src="https://i.imgur.com/cq3uPKz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
</p>
<p>
1. Connect to the VM via Remote Desktop Connection application on your PC</p>
2. Login with  username and password you created in step 1</p>
3. While in the VM, open <b>Microsoft Edge</b> or <b>Chrome</b> and click this link that includes the <a href="https://drive.google.com/drive/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6"> Installation Files  </a> for osTicket. </p>
4. Next open Control panel > Programs > Programs and Features > turn windows features on or off > then check internet information services > expand to world wide web services > application development features> check "CGI" and under "Common HTTP features" under world wide web services make sure everything is checked</p>
- To make sure it works, go to the edge browser to 127.0.0.1 in the url then it will load the windows Internet Information Services (IIS) page</p>
</p>
<br />

<p> Steps 3: <b>osTicket Installation Files</b>
<img src="https://i.imgur.com/7A6iquq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
</p>
<p>
1.  Open this link that includes the <a href="https://drive.google.com/drive/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6">  Installation Files </a> for osTicket. </p>
2. Download "PHPManagerforIIS" then install to VM</p>
3. Download "rewrite" then install to VM</p>
4. Go to files under the C: folder create a new folder called PHP</p>
5. Download PHP.zip and unzip in the created folder called PHP</p>
6. Download VC_redist and install</p>
7. Download MySQL and install</p>
</p>
<br />






