<p align="center">
  <img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket Logo"/>
</p>

# osTicket – Prerequisites and Installation

## Project Overview
This project demonstrates the deployment of an **osTicket help desk system** using **Microsoft Azure**, **Windows Server**, **IIS**, **PHP**, and **MySQL**.

The goal of this lab is to simulate a **real-world IT help desk environment** by installing, configuring, and validating a ticketing system commonly used by IT support teams. This project reflects tasks performed by **entry-level IT support and help desk professionals**.

---

## Environments and Technologies Used
- Microsoft Azure (Virtual Machines / Compute)
- Windows Server 2019 or 2022
- Remote Desktop Protocol (RDP)
- Internet Information Services (IIS)
- PHP
- MySQL
- HeidiSQL

---

## Operating System Used
- Windows Server 2019 or 2022 (Azure Virtual Machine)

---

## Prerequisites
- Active Azure subscription
- Windows Server 2019 or 2022 Virtual Machine
- Administrator access to the VM
- Internet access
- IIS installed with CGI enabled
- PHP 7.3 (legacy compatibility for osTicket lab)
- MySQL Server installed
- Azure Network Security Group allowing:
  - Port 80 (HTTP)
  - Port 3389 (RDP)

---

## Installation Steps

### Step 1: Connect to the Azure Virtual Machine
- Logged into the Windows Server VM using Remote Desktop.

<img src="https://github.com/user-attachments/assets/c1d9228b-310c-44e3-a733-975d6cd97051" />

---

### Step 2: Download Installation Files
- Downloaded `osTicket-Installation-Files.zip`
- Extracted files to the desktop inside the VM

<img src="https://github.com/user-attachments/assets/784f5d17-a604-41bf-90bc-92e6fea4dece" />

---

### Step 3: Install IIS with CGI Enabled
- Enabled IIS role
- Enabled CGI under:
  - World Wide Web Services → Application Development Features

<img src="https://github.com/user-attachments/assets/77040c5c-f0c4-4e38-a9df-91bfe9db8eb8" />

---

### Step 4: Install PHP and Dependencies
- Installed PHP Manager for IIS
- Installed IIS Rewrite Module
- Created `C:\PHP` directory
- Extracted PHP 7.3 into `C:\PHP`
- Installed Visual C++ Redistributable

<img src="https://github.com/user-attachments/assets/1f2c741b-e580-4914-93eb-b08217b7ceb2" />
<img src="https://github.com/user-attachments/assets/be7425e2-5ef5-4a06-bed1-72f370a638cb" />
<img src="https://github.com/user-attachments/assets/bcf6ee1d-bcc0-40d4-8bec-d4a74f31fbe4" />
<img src="https://github.com/user-attachments/assets/9e8dc479-12ad-49c7-8fdd-70afed2fafa1" />

---

### Step 5: Install and Configure MySQL
- Installed MySQL Server
- Completed standard configuration
- Created database credentials
- Installed HeidiSQL
- Created `osTicket` database

<img src="https://github.com/user-attachments/assets/d14be91b-0376-4161-adbd-27e7f7d5d476" />
<img src="https://github.com/user-attachments/assets/f0fd8725-a165-4637-a45e-1d52894ad229" />
<img src="https://github.com/user-attachments/assets/49c97f53-6f19-4211-9fba-558880c7ae7a" />

---

### Step 6: Configure IIS for PHP
- Opened IIS as Administrator
- Registered PHP (`php-cgi.exe`)
- Restarted IIS services

<img src="https://github.com/user-attachments/assets/aeee1c3d-9583-47ed-8917-206cf66d67f5" />
<img src="https://github.com/user-attachments/assets/2304b052-2b53-4526-b0c3-11be5376944d" />

---

### Step 7: Install osTicket
- Extracted osTicket files
- Copied `upload` folder to `C:\inetpub\wwwroot`
- Renamed folder to `osTicket`
- Restarted IIS

<img src="https://github.com/user-attachments/assets/8df9f981-abc8-4eac-8808-32fb07ebc318" />
<img src="https://github.com/user-attachments/assets/805f7f4e-a1f4-44c5-92a7-e439b2e81014" />

---

### Step 8: Enable Required PHP Extensions
Enabled the following extensions in PHP Manager:
- `php_imap.dll`
- `php_intl.dll`
- `php_opcache.dll`

<img src="https://github.com/user-attachments/assets/c11b0fd6-599d-410f-a12b-4817c6bc3914" />

---

### Step 9: Configure osTicket
- Renamed `ost-sampleconfig.php` to `ost-config.php`
- Assigned required permissions
- Completed web-based setup
- Verified successful installation

<img src="https://github.com/user-attachments/assets/342b22c3-6de7-41b9-98ed-e4354c2a720d" />
<img src="https://github.com/user-attachments/assets/f310c8b9-8d1c-4b06-86e2-9f809a9afe02" />
<img src="https://github.com/user-attachments/assets/b71ce4a9-928d-438e-9ee8-b8ae8c8102f6" />

---

## Troubleshooting & Lessons Learned
- IIS will not process PHP unless CGI is enabled
- Missing PHP extensions can block osTicket installation
- Proper file permissions are critical for configuration files
- IIS must be restarted after major configuration changes

---

## Skills Demonstrated
- Azure Virtual Machine deployment
- Windows Server administration
- IIS configuration
- PHP environment setup
- MySQL database creation and management
- Web application installation
- File and permission management
- IT documentation and troubleshooting

This project reflects tasks commonly performed by **IT support and help desk professionals** in real-world environments.
