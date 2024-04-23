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

STep1
We need to install the we will need to install the Internet Information Services (IIS). To install  Internet Information Service we will search for the Control Panel --> under programs select Uninstall a Program.. To install the Web Platform Installer we will search for the Control Panel --> under programs select Uninstall a Program.

<img width="859" alt="os picture 1" src="https://github.com/PeterCodyLeon/osticket-prereqs/assets/161895166/5ed96ee3-b08a-4e0d-b48d-779f6c7d4c12">


Step 2

After we've reached the next page, we can now select to Turn Windows features on or off. Then click the box to enable 'Internet Information Services' (IIS) from the available services.


<img width="802" alt="A os" src="https://github.com/PeterCodyLeon/osticket-prereqs/assets/161895166/4a93e7e1-a678-46b2-b6bf-3873bf9d8c51">




<p>
<img ![image](https://github.com/PeterCodyLeon/osticket-prereqs/assets/161895166/1471bb95-2457-4b52-b598-9d8403ff6b02)

<p>
Step 3
Enable php in IIS buy going clicking PHP manager and going to php and click php.cgi and click restart.

<img width="616" alt="ab" src="https://github.com/PeterCodyLeon/osticket-prereqs/assets/161895166/3fe3e6bc-a1b1-4d22-99f2-b8c6edc04609">


Step 4

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
Step 5
 Restart the IIS Server
Search for Internet Information Services (IIS) and select Open
Select Restart on the right-hand side
On the left side of the screen, select Desktop > Sites > Default Website > osTicket
On the right side of the screen, click “Browse *:80”
This should open osTicket in your web browser

<p>
<img width="801" alt="at" src="https://github.com/PeterCodyLeon/osticket-prereqs/assets/161895166/c5cb0eb2-2e3a-4ac2-bf8e-26fa0c49d271">

<img width="794" alt="at" src="https://github.com/PeterCodyLeon/osticket-prereqs/assets/161895166/414c2741-822a-4770-9239-2d030ecda869">




![image](https://github.com/PeterCodyLeon/osticket-prereqs/assets/161895166/40060ba4-efa6-4bd2-8413-0ae56e6e5b9e)

Step 6

Open Windows Explorer and select C: > inetpub > wwwroot > osTicket > include
Rename the following file:
From: ost-SAMPLEconfig.php
To: ost-config.php

Step 7

 Assign Permissions to ost-config.php
 
Right-click ost-config.php

Open Properties > Security > Advanced > Permissions

Select Disable Inheritance > Remove all inherited permissions from this object

![image](https://github.com/PeterCodyLeon/osticket-prereqs/assets/161895166/4fc864ef-b87d-47bb-9486-56f7fa1c7c91)


Step 8
Next , select Add select Principal, type in "everyone" > select Check Names > select OK
Allow everyone full control (check all boxes) > Select apply > OK

![image](https://github.com/PeterCodyLeon/osticket-prereqs/assets/161895166/6100416a-1ea9-4f81-bdc6-e49e6140ba6f)

![image](https://github.com/PeterCodyLeon/osticket-prereqs/assets/161895166/3fda99b7-596d-4cc0-95b2-acea494d80a1)































































Step 9

Continue Setting Up osTicket in Browser
Go back to the browser and click Continue
Name: Helpdesk
Email: whichever email you want
First Name: your first name
Last Name: your last name
Email Address: whichever email you want (needs to be different from the Helpdesk's default email)
Username: Peter Leon
Password: Enter password of choice as long as it's strong to protect your information

![image](https://github.com/PeterCodyLeon/osticket-prereqs/assets/161895166/9187111b-3271-40e0-9881-4e17940c0edb)


 ![image](https://github.com/PeterCodyLeon/osticket-prereqs/assets/161895166/cf26d38d-2c86-490b-b172-771a37f7a7d4)


 


Step 10: Download and Install HeidiSQL

Head to osTicket Installation Files link

Download and install HeidiSQL

Open HeidiSQL > Select "New" at the bottom-left corner of the screen
User: root

Password: Password of your choice
Select Open

On the left side, right-click Unnamed > select Create New > Database
Name it “osTicket” and select OK

![image](https://github.com/PeterCodyLeon/osticket-prereqs/assets/161895166/dac1c4ae-9ec4-4805-b7d8-b080bb9d3ee8)


Step 11 : Continue Setting Up osTicket by Filling Out the Fields
Go back to the browser
MySQL Database: osTicket (the one you just created in HeidiSQL)
MySQL Username: root
MySQL Password of personal choice
Finally, click Install Now

 ![image](https://github.com/PeterCodyLeon/osticket-prereqs/assets/161895166/e75e715a-1bda-41c3-be50-a3a5d1f03a9c)


Now you should see congratualions on installing osticket.

![image](https://github.com/PeterCodyLeon/osticket-prereqs/assets/161895166/27886b71-e4e4-40b9-a9b5-d3b1f420a89b)





<img 
<p>
At this point you should have downloaded latest version of osTicket. Uncompress the files and upload files and directories in upload folder to a directory of your choice on your server. For example /osticket/, /helpdesk/ or /support/ depending on your preference. Basic knowledge of using FTP is a plus at this stage. If you don’t know how to use FTP, we would recommend you read the documentation supplied with your FTP client and learn the basics of uploading and setting permissions on files.
</p>
<br />Once osTicket has been installed you need to further configure it via admin panel before it is fully usable. Only staff with admin's privileges can access the admin panel. Please use the username and password created during the install process.

Email Setup
-----------

Setting up your system to accept emails varies from system to system and your personal preference. osTicket allows you to route unlimited number of emails as incoming tickets. For detailed instruction please see :doc:`Email Settings Guide <Email Settings>`.


![image](https://github.com/PeterCodyLeon/osticket-prereqs/assets/161895166/9f5bd5d8-b2f7-4761-a958-45d8389ce1a3)


