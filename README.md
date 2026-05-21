# osTicket-Installation-and-Configuration
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Installation</h1>
This tutorial outlines the installation of the open-source help desk ticketing system osTicket. This is a condensed and simplified version of the install, but all of the steps follow documentation supplied by osTicket on their github https://github.com/osTicket/osTicket-1.7.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure Virtual Machines (Compute)
- Remote Desktop (RDP)
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 11</b> (25H2)

<h2>Prerequisites</h2>

<img width="800" height="500" alt="pre1" src="https://github.com/user-attachments/assets/d189709a-e5bf-4557-ae2f-0cd3993f6b9d" />

<p>
Created a Microsoft Azure account and accessed the Azure Portal dashboard.</p>

<img width="800" height="500" alt="pre2" src="https://github.com/user-attachments/assets/09a2b816-5ea2-4419-88fb-376d640a41fc" />

Navigated to the Virtual Machines service, selected Create, and deployed a new virtual machine instance.

<img width="800" height="500" alt="OS-1" src="https://github.com/user-attachments/assets/7f481086-b1ee-43b3-85c2-664659e37590" />

Created a virtual machine with the Windows 11 Pro Image and user/pass of choice.

<img width="800" height="800" alt="OS-3" src="https://github.com/user-attachments/assets/0d40e64b-9d2c-4a47-ab32-7c628ec26d54" />
<img width="446" height="411" alt="OS-4" src="https://github.com/user-attachments/assets/099bcfa7-8db5-4251-b515-3716f1d0d54c" />

Used the virtual machine’s public IP address to establish a Remote Desktop Protocol (RDP) connection from a local machine.
</p>
<p></p>
<h2>Installation Steps</h2>
<p>
All of the remaining setup steps were completed inside the virtual machine. I downloaded the osTicket installation files from the official website, extracted them to the desktop, and started configuring the prerequisites needed for the application to run properly.

To host osTicket locally as a web application, I installed Internet Information Services (IIS) and enabled the CGI feature through Windows Features. CGI is required for IIS to process the PHP files used by osTicket.

Before enabling IIS and CGI, entering the loopback address (localhost / 127.0.0.1) in the browser did not display anything because the web server services were not yet configured. After enabling the required features, the default IIS webpage loaded successfully, confirming that the local web server environment was running correctly.
</p>
<img width="3370" height="1384" alt="OS-5" src="https://github.com/user-attachments/assets/58d0e007-472a-4d4b-86da-924bbe685db8" />
<img width="413" height="368" alt="os-6 3" src="https://github.com/user-attachments/assets/f103cece-deb3-4a2e-b7bc-0474741f6159" />
<img width="408" height="366" alt="os-6 4" src="https://github.com/user-attachments/assets/1be916b8-1f8d-42ff-9cf4-f8aec79f5031" />
<img width="600" height="600" alt="OS-6 1" src="https://github.com/user-attachments/assets/b2194b9f-96c6-46f0-b9c1-4ebe789de33c" />
<img width="600" height="600" alt="os-7" src="https://github.com/user-attachments/assets/4da421a1-08c8-4c8b-940d-879a84e26865" />


<p>
At this stage, I extracted and installed the additional backend resources required to support the osTicket environment, including the PHP components needed for the application to run properly on the web server.

I also installed HeidiSQL, which will be used to manage the MySQL database connection for osTicket. This database setup allows osTicket to communicate with the backend database through the PHP environment and store ticketing system data correctly.
</p>
<img width="1000" height="699" alt="os-8" src="https://github.com/user-attachments/assets/5f162aca-fa62-403b-8fbf-c12f02b6dad0" />
<img width="1000" height="652" alt="os-9" src="https://github.com/user-attachments/assets/018ee517-cf23-4d83-ae33-72ec34b572f3" />
<img width="1000" height="630" alt="os-12" src="https://github.com/user-attachments/assets/f0011e0b-837d-42dc-871c-4e113fcd5ab3" />
<img width="1000" height="633" alt="os-13" src="https://github.com/user-attachments/assets/e428ef61-c9dc-47d8-82ca-76c5d9431d76" />
<img width="1380" height="624" alt="os-21" src="https://github.com/user-attachments/assets/c5ae1b7e-a301-4795-a1b8-b7b5f19b16a0" />
<img width="513" height="387" alt="os-23" src="https://github.com/user-attachments/assets/94977b9e-b3b0-418c-94c8-b302f0ffbc34" />
<img width="929" height="587" alt="os-26" src="https://github.com/user-attachments/assets/ba29ab1f-f3b3-4822-bedb-0836f09403ec" />

<p>
The final steps are mostly about finishing the setup inside osTicket. This includes configuring the main system settings and creating the administrator account so you can access and manage the platform.

After that, I connected osTicket to the backend database by entering the required credentials and testing the connection. Once that was complete, everything was successfully linked, and the system was fully set up and ready to use.
<img width="1542" height="1287" alt="os-24" src="https://github.com/user-attachments/assets/f52ecbd0-fd39-4d80-82ca-15b360c05182" />
<img width="1451" height="760" alt="os-25" src="https://github.com/user-attachments/assets/2a764a2c-a20d-4168-ab28-4a960c0c5531" />

</p>

<br />
