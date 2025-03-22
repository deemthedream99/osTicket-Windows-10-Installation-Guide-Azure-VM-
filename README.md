# osTicket Windows 10 Installation

## Overview
This project documents the setup and configuration of an osTicket helpdesk system in an Azure Virtual Machine (VM) running Windows 10. The guide covers installing and configuring IIS with CGI, PHP, MySQL, and required dependencies, ensuring a functional osTicket environment.

## Components
- Primary System: Windows 10 (Azure Virtual Machine)
- Hypervisor: Azure Virtual Machine

## Steps Taken
1. Created an Azure VM running Windows 10 with 4 vCPUs.
2. Installed IIS with CGI support to enable web hosting.
3. Installed PHP and MySQL, along with required dependencies:
    - PHP Manager for IIS
    - IIS Rewrite Module
    - Microsoft Visual C++ Redistributable
4. Configured IIS for osTicket:
    - Registered PHP with IIS
    - Unzipped and placed osTicket files in C:\inetpub\wwwroot\osTicket
5. Enabled necessary PHP extensions (php_imap.dll, php_intl.dll, php_opcache.dll).
6. Set up osTicket via the web interface, providing:
    - Database: MySQL 5.5.62
    - Credentials: root/root
    - Helpdesk name and default email
7. Installed HeidiSQL to manage the MySQL database.
8. Finalized installation by renaming and securing the ost-config.php file.
9. Cleaned up setup files and ensured proper permissions for security.

## Verification Screenshots
![localhost Homepage](https://github.com/user-attachments/assets/56036c65-bcd7-4d77-84ba-ed7fc501e4c7)
![osTicket Homepage](https://github.com/user-attachments/assets/31966e4e-c93a-41c5-abd8-2c7b1a37171d)
![osTicket Homepage (after enabling extensions)](https://github.com/user-attachments/assets/a36c4c1f-4ce7-4910-8296-ffdc998f2665)
![osTicket Installation](https://github.com/user-attachments/assets/0dc0ede4-c84f-4cdb-8d64-0bb41e3196d0)
![Installation Complete!](https://github.com/user-attachments/assets/4861fd2c-2a00-446c-8910-5181c19cc073)
