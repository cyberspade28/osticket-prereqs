<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />
Setup a Virtual Machine in Azure
Install the osTicket requirements
Install osTicket itself
Do the after-installation configuration of osTicket
Explore osTicket as a Help Desk Professional
Create, interact, and close tickets
Clean up Virtual Environment in Azure



<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

Windows 10, 4 vCPUs

<h2>List of Prerequisites</h2>

Active Azure subscription

Windows Server 2019 or 2022 VM

Administrator access to the VM

IIS installed

PHP 8.0+ installed

MySQL Server installed

Internet access

Open ports 80 and 3389 in Azure NSG

<h2>Installation Steps</h2>

<p>
 />
</p>
<p>
Log into the VM with Remote Desktop

Within the VM (osticket-vm), download the osTicket-Installation-Files.zip and unzip it onto your desktop. The folder should be called “osTicket-Installation-Files”
We will use the files in this folder to install osTicket and some of the dependencies.

Install / Enable IIS in Windows WITH CGI
World Wide Web Services -> Application Development Features -> [X] CGI

From the “osTicket-Installation-Files” folder, install PHP Manager for IIS (PHPManagerForIIS_V1.5.0.msi)


Create the directory C:\PHP

From the “osTicket-Installation-Files” folder, unzip PHP 7.3.8 (php-7.3.8-nts-Win32-VC15-x86.zip) into the “C:\PHP” folder

From the “osTicket-Installation-Files” folder, install VC_redist.x86.exe.

From the “osTicket-Installation-Files” folder, install MySQL 5.5.62 (mysql-5.5.62-win32.msi</p>
<br />

<p>
Log into the VM with Remote Desktop

<img width="2560" height="1440" alt="image" src="https://github.com/user-attachments/assets/c1d9228b-310c-44e3-a733-975d6cd97051" />
<img width="2560" height="1440" alt="image" src="https://github.com/user-attachments/assets/784f5d17-a604-41bf-90bc-92e6fea4dece" />

<img width="2560" height="1440" alt="Screenshot (9)" src="https://github.com/user-attachments/assets/77040c5c-f0c4-4e38-a9df-91bfe9db8eb8" />

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
