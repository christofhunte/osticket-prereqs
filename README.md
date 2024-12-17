<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop (Microsoft Remote Desktop)
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- IIS installed with CGI
- MySQL
- PHP registered from within IIS
- Extensions within PHP manager are enabled
- Hedi SQL and MySQL on osTicket are set up

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/wuSQPWr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<img src="https://i.imgur.com/gcaaTSd.png" height="80%" width="80%" alt="Disk Sanitization Steps"/> 
<p>
The first thing I did was go into Azure cloud and create a Windows 10 virtual machine. I made sure to run a VM with 2 vcpus to ensure the server could handle all of the files. I also set the machine to create its own virtual network and set the port to RDP. After the VM was set up I took the Public IP address created by the VM, installed and opened Microsoft Remote desktop to launch the Windows Server. I logged in with VM user account and Uploaded the osTicket installation files needed onto the server desktop and extracted all the fies.
</p>
<br />

<p>
<img src="https://i.imgur.com/h4cywGY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/OHhHSbw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
The next thing I did was install IIS with CGI. Then I installed the sofware in the osTicket-Installation-Files including the PHP Manager for IIS, the Rewrite Module, MySQL, etc. I also created a PHP folder on the C drive and extracted the PHP 7.3.8 contents from the "osTicket" folder into the PHP folder. I launched the MySQL Configuration Wizard and created a username and password. I then registered the PHP in the IIS. I then lauched the osTicket zip file in the folder and copied the upload folder and pasted it into the inetpub folder in the C drive and renamed it into osTicket. 
</p>
<br />

<p>
<img src="https://i.imgur.com/3qhgrG7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
I then browsed the osTicket site and enabled extensions that were necessary for the site to work in the PHP manager such as php_imap.dll, php_intl.dll and php_opcache.dll. 
</p>
<br />
