<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


 
<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Amazon Web Services(Virtual Machines/Computer)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

1- PHP 8.2/8.1 for Windows Server

2- MySQL 8.0 for Windows Server: You’ll need a MySQL database with a valid user, password, and hostnam

3- MariaDB 10.11 for Windows Server

4- PHP Manager 2 for IIS (makes managing PHP on IIS much easier
 
<h2>Installation Steps</h2>


We need to install the we will need to install the Internet Information Services (IIS). To install  Internet Information Service we will search for the Control Panel --> under programs select Uninstall a Program.. To install the Web Platform Installer we will search for the Control Panel --> under programs select Uninstall a Program.

<img width="859" alt="os picture 1" src="https://github.com/PeterCodyLeon/osticket-prereqs/assets/161895166/5ed96ee3-b08a-4e0d-b48d-779f6c7d4c12">



After we've reached the next page, we can now select to Turn Windows features on or off. Then click the box to enable 'Internet Information Services' (IIS) from the available services.


<img width="802" alt="A os" src="https://github.com/PeterCodyLeon/osticket-prereqs/assets/161895166/4a93e7e1-a678-46b2-b6bf-3873bf9d8c51">




<p>
<img ![image](https://github.com/PeterCodyLeon/osticket-prereqs/assets/161895166/1471bb95-2457-4b52-b598-9d8403ff6b02)

<p>

Enable php in IIS buy going clicking PHP manager and going to php and click php.cgi and click restart.

<img width="616" alt="ab" src="https://github.com/PeterCodyLeon/osticket-prereqs/assets/161895166/3fe3e6bc-a1b1-4d22-99f2-b8c6edc04609">



Download osTicket from the Installation Files Folder
Extract and copy “upload” folder to c:\inetpub\wwwroot
Within c:\inetpub\wwwroot, Rename “upload” to “osTicket”

![image](https://github.com/PeterCodyLeon/osticket-prereqs/assets/161895166/65bdc271-36d3-4aa8-8ed4-3a68d2a7cd38)


</p>
<br />

<p>"/>
</p>

</p>
<br />

 Restart the IIS Server
Search for Internet Information Services (IIS) and select Open
Select Restart on the right-hand side
On the left side of the screen, select Desktop > Sites > Default Website > osTicket
On the right side of the screen, click “Browse *:80”
This should open osTicket in your web browser

<p>
<img width="801" alt="at" src="https://github.com/PeterCodyLeon/osticket-prereqs/assets/161895166/c5cb0eb2-2e3a-4ac2-bf8e-26fa0c49d271">

<img width="794" alt="at" src="https://github.com/PeterCodyLeon/osticket-prereqs/assets/161895166/414c2741-822a-4770-9239-2d030ecda869">

![image](https://github.com/PeterCodyLeon/osticket-prereqs/assets/161895166/6b53e64a-4087-408c-bea2-4466cd6e3ccf)


 
<img 
<p>
At this point you should have downloaded latest version of osTicket. Uncompress the files and upload files and directories in upload folder to a directory of your choice on your server. For example /osticket/, /helpdesk/ or /support/ depending on your preference. Basic knowledge of using FTP is a plus at this stage. If you don’t know how to use FTP, we would recommend you read the documentation supplied with your FTP client and learn the basics of uploading and setting permissions on files.
</p>
<br />Once osTicket has been installed you need to further configure it via admin panel before it is fully usable. Only staff with admin's privileges can access the admin panel. Please use the username and password created during the install process.

Email Setup
-----------

Setting up your system to accept emails varies from system to system and your personal preference. osTicket allows you to route unlimited number of emails as incoming tickets. For detailed instruction please see :doc:`Email Settings Guide <Email Settings>`.


![image](https://github.com/PeterCodyLeon/osticket-prereqs/assets/161895166/9f5bd5d8-b2f7-4761-a958-45d8389ce1a3)


