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
Within the VM (osticket-vm), download the osTicket-Installation-Files.zip and unzip it onto your desktop. The folder should be called “osTicket-Installation-Files”
We will use the files in this folder to install osTicket and some of the dependencies.

<img width="2560" height="1440" alt="image" src="https://github.com/user-attachments/assets/784f5d17-a604-41bf-90bc-92e6fea4dece" />
Install / Enable IIS in Windows WITH CGI
World Wide Web Services -> Application Development Features -> [X] CGI

<img width="2560" height="1440" alt="Screenshot (9)" src="https://github.com/user-attachments/assets/77040c5c-f0c4-4e38-a9df-91bfe9db8eb8" />

</p>
From the “osTicket-Installation-Files” folder, install PHP Manager for IIS (PHPManagerForIIS_V1.5.0.msi)

<img width="2560" height="1440" alt="Screenshot (10)" src="https://github.com/user-attachments/assets/1f2c741b-e580-4914-93eb-b08217b7ceb2" />
</p>
<br />

From the “osTicket-Installation-Files” folder install the Rewrite Module (rewrite_amd64_en-US.msi)
<img width="2560" height="1440" alt="Screenshot (13)" src="https://github.com/user-attachments/assets/be7425e2-5ef5-4a06-bed1-72f370a638cb" />

Create the directory C:\PHP
<img width="2560" height="1440" alt="Screenshot (14)" src="https://github.com/user-attachments/assets/bcf6ee1d-bcc0-40d4-8bec-d4a74f31fbe4" />
From the “osTicket-Installation-Files” folder, unzip PHP 7.3.8 (php-7.3.8-nts-Win32-VC15-x86.zip) into the “C:\PHP” folder

<img width="2560" height="1440" alt="Screenshot (15)" src="https://github.com/user-attachments/assets/9e8dc479-12ad-49c7-8fdd-70afed2fafa1" />

</p>From the “osTicket-Installation-Files” folder, install VC_redist.x86.exe.

<br /><img width="2560" height="1440" alt="Screenshot (16)" src="https://github.com/user-attachments/assets/6e1d6638-a1bb-4675-b469-64d2e332dee4" />
From the “osTicket-Installation-Files” folder, install MySQL 5.5.62 (mysql-5.5.62-win32.msi)
Typical Setup ->
Launch Configuration Wizard (after install) ->
Standard Configuration ->
Username: root
Password: root

<img width="2560" height="1440" alt="Screenshot (17)" src="https://github.com/user-attachments/assets/d14be91b-0376-4161-adbd-27e7f7d5d476" />
<img width="2560" height="1440" alt="Screenshot (18)" src="https://github.com/user-attachments/assets/f0fd8725-a165-4637-a45e-1d52894ad229" />
Open IIS as an Admin
<img width="2560" height="1440" alt="Screenshot (19)" src="https://github.com/user-attachments/assets/aeee1c3d-9583-47ed-8917-206cf66d67f5" />
Register PHP from within IIS (PHP Manager -> C:\PHP\php-cgi.exe)
<img width="2560" height="1440" alt="Screenshot (20)" src="https://github.com/user-attachments/assets/2304b052-2b53-4526-b0c3-11be5376944d" />
Reload IIS (Open IIS, Stop and Start the server)
<img width="2560" height="1440" alt="Screenshot (22)" src="https://github.com/user-attachments/assets/f273456a-07f4-4c1b-94d3-f2344a577547" />
<img width="2560" height="1440" alt="Screenshot (23)" src="https://github.com/user-attachments/assets/e5a3cd6f-8920-4911-ab8c-e8f0c3d0869b" />
Install osTicket v1.15.8
From the “osTicket-Installation-Files” folder, unzip “osTicket-v1.15.8.zip” and copy the “upload” folder into “c:\inetpub\wwwroot”
Within “c:\inetpub\wwwroot”, Rename “upload” to “osTicket”
<img width="2560" height="1440" alt="Screenshot (24)" src="https://github.com/user-attachments/assets/8df9f981-abc8-4eac-8808-32fb07ebc318" />
<img width="2560" height="1440" alt="Screenshot (25)" src="https://github.com/user-attachments/assets/805f7f4e-a1f4-44c5-92a7-e439b2e81014" />
<img width="2560" height="1440" alt="Screenshot (26)" src="https://github.com/user-attachments/assets/a6fabf15-90ca-4c1c-b45a-7931f5c96772" />
Reload IIS (Open IIS, Stop and Start the server)
<img width="2560" height="1440" alt="Screenshot (27)" src="https://github.com/user-attachments/assets/48633f15-e8b5-43d0-baa0-af05ab8493cd" />



