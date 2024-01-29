<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Azure Subscription - Ensure you have an active Microsoft Azure subscription. If not, create one at Azure Portal.
- Resource Group - Create an Azure Resource Group to organize and manage the resources for osTicket.
- Azure Virtual Machine - Set up an Azure Virtual Machine (VM) to host osTicket. Choose a Windows Server VM.
- Microsoft Remote Desktop - Install Microsoft Remote Desktop on your local machine to connect to the Azure VM.
- IIS (Internet Information Services) - Enable IIS on the Azure VM. This will serve as the web server for osTicket.
- SSL Certificate (Optional) - If you plan to use HTTPS, obtain an SSL certificate. You can use Azure's own certificate service or a third-party provider.

  
<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/tMcYLQi.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  Create a Virtual Machine:

In the Azure Portal, navigate to "Virtual machines" and create a new VM.
Choose a Windows Server image, configure settings, and define networking options.
</p>

<p>Remote Desktop Connection:

Connect to the Azure VM using Microsoft Remote Desktop. Retrieve the VM's public IP address for connection.
</p>
<br />

<p>
<img src="https://i.imgur.com/pmRgfgF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>Enable IIS:
On the Azure VM, open the "Server Manager."
Select "Manage" > "Add Roles and Features" and install the IIS role.
</p>

<p>
  Download osTicket:

Use a web browser on the Azure VM to download the latest version of osTicket.</p>

<p>Extract and Move Files:

Extract the osTicket archive and move the files to the C:\inetpub\wwwroot directory (default IIS web root).</p>

<p>Configure Permissions:

Adjust permissions on the osTicket directory to ensure IIS has necessary read and write access.
</p>

<p>
  Set Up Database:
Use Microsoft SQL Server or another supported database server on the Azure VM.
Create a new database for osTicket and note down the connection details.
</p>

<p>
  Navigate to Installer:
Open a web browser on the Azure VM and navigate to http://localhost or use the VM's public IP address.
Follow the on-screen instructions to complete the osTicket installation.
</p>
<br />

<p>
<img src="https://i.imgur.com/g9i3fPL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Admin Panel Setup:

Access the osTicket admin panel using the administrator credentials you created during the installation.
Customize settings, configure email, and set up departments as needed.</p>
  
<p>Test and Secure:

Create a sample ticket to ensure that osTicket is working correctly.
Implement security measures, such as using HTTPS, securing sensitive directories, and keeping the osTicket software up to date.</p>

<p>
  Secure Remote Desktop:
Implement security measures for Remote Desktop, such as using Network Level Authentication (NLA) and strong authentication methods.</p>
<br />
