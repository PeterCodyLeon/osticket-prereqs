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

<p>
<img ![image](https://github.com/PeterCodyLeon/osticket-prereqs/assets/161895166/1471bb95-2457-4b52-b598-9d8403ff6b02)

<p>

Enable php in IIS buy going clicking PHP manager and going to php and click php.cgi and click restart.

![image](https://github.com/PeterCodyLeon/osticket-prereqs/assets/161895166/65bdc271-36d3-4aa8-8ed4-3a68d2a7cd38)


Download osTicket from the Installation Files Folder
Extract and copy “upload” folder to c:\inetpub\wwwroot
Within c:\inetpub\wwwroot, Rename “upload” to “osTicket”

</p>
<br />

<p>"/>
</p>
 </p>


</p>
<br />

<p>
<img 
<p>
At this point you should have downloaded latest version of osTicket. Uncompress the files and upload files and directories in upload folder to a directory of your choice on your server. For example /osticket/, /helpdesk/ or /support/ depending on your preference. Basic knowledge of using FTP is a plus at this stage. If you don’t know how to use FTP, we would recommend you read the documentation supplied with your FTP client and learn the basics of uploading and setting permissions on files.
</p>
<br />Once osTicket has been installed you need to further configure it via admin panel before it is fully usable. Only staff with admin's privileges can access the admin panel. Please use the username and password created during the install process.

Email Setup
-----------

Setting up your system to accept emails varies from system to system and your personal preference. osTicket allows you to route unlimited number of emails as incoming tickets. For detailed instruction please see :doc:`Email Settings Guide <Email Settings>`.


![image](https://github.com/PeterCodyLeon/osticket-prereqs/assets/161895166/9f5bd5d8-b2f7-4761-a958-45d8389ce1a3)

Post Installation Setup
-----------

In addition to emails, clients/users can also use an online form to create tickets. Help topics helps maps online inquiries to a department and assigns priority without the need for the user to select a department or/and ticket priority. This gives you ability to route inquiries without exposing internal departments.

Departments
-----------

Departments are used to categorize incoming tickets and also as access mask for staff members. For example you can restrict staff's tickets access based on departments. To manage departments go to the **Departments** tab in the **Admin Panel**.

Staff Members
-------------

OsTicket allows you to add unlimited number of representatives to the system. Each staff member is assigned to a group and a department which determines the level of permission. Every staff account can be of type 'Admin' or 'Staff'.

System Preferences
------------------

To disable or change system settings, go to Settings Tab in **Admin Panel**
