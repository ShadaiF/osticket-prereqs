<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the installation of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Computer)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)


<h2>Installation Steps</h2>

<p> Step 1: <b> Create Virtual Machine in Azure </b> </p>

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

<p> Step 2: <b> Installation </b> </p>
<img src="https://i.imgur.com/cq3uPKz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
</p>
<p>
1. Connect to the VM via <b>"Remote Desktop Connection"</b> application on your PC</p>
2. Login with username and password you created in step 1</p>
3. While in the VM, open <b>Microsoft Edge</b> or <b>Chrome</b> and click this link that includes the <a href="https://drive.google.com/drive/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6"> Installation Files  </a> for osTicket. </p>
4. Next open Control panel > Programs > Programs and Features > turn windows features on or off > then check Internet Information Services > expand to world wide web services > application development features > check "CGI" and under "Common HTTP features" under world wide web services make sure everything is checked</p>
5. To make sure this worked, open the browser you used and enter 127.0.0.1 in the url, it will load the Windows Internet Information Services (IIS) page</p>
</p>
<br />

<p> Steps 3: <b>osTicket Installation Files</b>
<img src="https://i.imgur.com/7A6iquq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
</p>
<p>
1.  Open this link that includes the <a href="https://drive.google.com/drive/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6">  Installation Files </a> for osTicket. </p>
2. Download "PHPManagerforIIS" and install to VM</p>
3. Download "rewrite" and install to VM</p>
4. Go to files under the <b>C:</b> folder create a new folder called "PHP"</p>
5. Download "PHP.zip" and unzip in the folder you created: "PHP"</p>
6. Download "VC_redist" and install</p>
7. Download "MySQL" and install</p>
</p>
<br />


<p> Steps 4: <b>MySQL and PHP Manager</b>
<img src="https://i.imgur.com/VXIYz8O.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
</p>
<p>
1. Launch SQL > Standard Config  </p>
2. Write down username: <b>root</b> and password: <b>Password1</b></p>
3. Click Execute and Finish </p>
4. Launch IIS as admin > open PHP Manager</p>
5. Register new PHP version and find the <b>C:</b> in the PHP folder in the new window </p>
6. Click PHP-CGI</p>
<b>* REMINDER * Hit restart on the top right and refresh server </b></p>
</p>
<br />

<p> Steps 5: <b>MySQL and PHP Manager</b> </p>
<img src="https://i.imgur.com/GG3k1RC.png" height="60%" width="60%" alt="Disk Sanitization Steps"/> <img src="https://i.imgur.com/0LO7bM5.png" height="60%" width="60%" alt="Disk Sanitization Steps"/>
</p> 
<p>
1. Launch SQL > Standard Config  </p>
2. Write down username: <b>root</b> and password: <b>Password1</b></p>
3. Click Execute and Finish </p>
4. Launch IIS as admin > open PHP Manager</p>
5. Register new PHP version and find the <b>C:</b> in the PHP folder in the new window </p>
6. Click PHP-CGI</p>
<b>* REMINDER * Hit restart on the top right and refresh server </b></p>
</p>
<br />

<p> Steps 6: <b>Extention</b></p>
<img src="https://i.imgur.com/usAABmr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
</p>
<p>
1. Expand the sites folder on the top left > expand until you see osTicket folder > hit browse link on the right hand side </p>
2. Go back to IIS > PHP manager > click on Enable or Disable Extensions</p>
3. Enable "php_imap.dll"</p>
4. Enable "php_intl.dll"</p>
5. Enable "php_opcache.dll"</p>
6. Go back to browser and refresh until some appear green</p>
</p>
<br />

<p> Step 7: <b> Security </b> </p>

<img src="https://i.imgur.com/C12gU9C.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
</p>
<p>
1. Open File Explorer > C: > inetpub > wwwroot > osTicket > Include > rename file from <b>ost-sampleconfig</b> to <b>ost-config</b> </p>
2. Right click on the ost-config file and click Properties > Security > Advanced > Disable inheritance </p>
3. Select a principal > type "Everyone" </p>
6. Check the name and add then apply and ok </p>
7. Basic permissions as full control >apply > ok </p>
</p>
<br />

<p> Step 8: <b> osTicket Browser Setup </b> </p>

<img src="https://i.imgur.com/yPngR72.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
</p>
<p>
1. Click back over to browser and contine with the osTicket setup</p>
2. After saving the usernames and passwords to a note pad</p>
3. Download the MYSQL database exe "HediSQL"</p>
4. Run HediSQL and install </p>
5. Launch > click new on the bottom left</p>
6. Username as <b>root</b> and password as <b>Password1</b></p>
7. Right click on "unnamed" at the top > create database</p>
8. Name it "osTicket"</p>
9. Go back to browser click install now after filling everything in, MySQL Database: osTicket</p>
10. Go to c: > inetpub > wwwroot > osTicket > right click on the setup folder and delete it</p>
11. Go into the include folder and edit the ost-config php and properties then under security go to advanced and change to read and execute only</p>
12.  <a href="http://localhost/osTicket/"> Admin Access osTicket </a></p>
13. <a href="http://localhost/osTicket/"> End Users osTicket URL </a></p>
</p>
<br />

