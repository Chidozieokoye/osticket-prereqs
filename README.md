<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

https://youtu.be/DZESWgr-4NU

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

Download the osTicket-Installation-Files

Install / Enable IIS in Windows WITH CG

Install PHP Manager for IIS and Rewrite Module

Create the directory C:\PHP and unzip PHP 7.3.8 into it

Install VC_redist.x86.exe and MySQL 5.5.62

Open IIS as an admin and register PHP

Reload IIS and Install osTicket v1.15.8 

Reload IIS, load osTicket, and enable disabled extensions

Rename ost-sampleconfig.php file to ost-config.php and assign permission to it

Install HeidiSQL and create a new database called “osTicket

Update osTicket in the web browser

<h2>Installation Steps</h2>

<h2>Install / Enable IIS in Windows WITH CGI</h2>

<p>
<img src="https://i.imgur.com/qN7NBiJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
When installing osTicket on Windows, you need a web server to handle requests. Windows comes with IIS (Internet Information Services), which is a built-in web server used for hosting websites and applications. However, since IIS does not natively support PHP, we need to enable CGI (Common Gateway Interface) to allow IIS to execute PHP scripts. Since osTicket is a PHP-based ticketing system, it cannot run directly on IIS without an interpreter. The CGI module (specifically FastCGI in modern versions of IIS) enables PHP scripts to execute efficiently. PHP in the other hand is a server-side scripting language used to create dynamic web applications. osTicket is built using PHP, meaning IIS needs a way to execute PHP scripts when users interact with the system.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
