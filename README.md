<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
In this lab, I started by downloading the osTicket installation files and configuring IIS with CGI support. I then installed PHP along with the required modules, set up MySQL, and registered PHP in IIS before proceeding with the installation of osTicket v1.15.8. After the installation, I reloaded IIS, enabled the necessary PHP extensions, and renamed the osTicket configuration file, ensuring it had the correct permissions. Next, I used HeidiSQL to create a new database for osTicket, and I completed the installation through the web browser. For a more detailed walkthrough, please check out the video demonstration below.<br />


<h2>Video Demonstration</h2>

https://youtu.be/DZESWgr-4NU

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Computer)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

1. Download the osTicket-Installation-Files

2. Install / Enable IIS in Windows WITH CG

3. Install PHP Manager for IIS and Rewrite Module

4. Create the directory C:\PHP and unzip PHP 7.3.8 into it

5. Install VC_redist.x86.exe and MySQL 5.5.62

6. Open IIS as an admin and register PHP

7. Reload IIS and Install osTicket v1.15.8

8. Reload IIS, load osTicket, and enable disabled extensions

9. Rename ost-sampleconfig.php file to ost-config.php and assign permission to it

10. Install HeidiSQL and create a new database called “osTicket

11. Update osTicket in the web browser

<h2>Installation Steps</h2>

<h2>Install / Enable IIS in Windows WITH CGI</h2>

<p>
<img src="https://i.imgur.com/qN7NBiJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In this step, IIS (Internet Information Services), which is Windows' built-in web server, is installed and configured with CGI (Common Gateway Interface) to enable support for executing PHP scripts. Since IIS does not natively process PHP, enabling CGI (specifically FastCGI) allows IIS to interpret and run PHP-based applications like osTicket, ensuring proper communication between the web server and the PHP interpreter.
</p>
<br />

<h2>Open IIS as an admin and register PHP</h2>

<p>
<img src="https://i.imgur.com/cVJmcVS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
When you open IIS as an administrator and register PHP, you’re configuring IIS to handle and process PHP files, as IIS does not support PHP natively. By running IIS with administrative privileges, you ensure you have the necessary access to modify server settings. Registering PHP involves associating the .php file extension with the appropriate handler, typically FastCGI, which allows IIS to pass PHP requests to the PHP interpreter for execution. This step enables IIS to process dynamic content generated by PHP scripts and ensures applications like osTicket, which rely on PHP, can run smoothly on the server. It also optimizes performance by maintaining the PHP process in memory, reducing overhead and improving response times for user requests.
</p>
<br />

<h2>Install HeidiSQL and create a new database called “osTicket</h2>

<p>
<img src="https://i.imgur.com/Re8kBiY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
When you install HeidiSQL and create a new database called “osTicket”, you're setting up a powerful database management tool that provides a graphical interface to easily interact with MySQL or MariaDB databases. After installation, you connect HeidiSQL to your database server, providing it with the necessary credentials (server address, username, password) to access the server. Once connected, you create a new database specifically for osTicket, which will house all its data such as user information, tickets, system settings, and logs. This process is essential for osTicket to function properly, as the system relies on this dedicated database to store, retrieve, and manage all the data that powers the ticketing operations. Creating this database ensures that osTicket has a clean and organized storage structure to handle requests and maintain smooth operations.
</p>
<br />
