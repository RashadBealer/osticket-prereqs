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
Begin by visiting the official osTicket website or GitHub repository and download the latest stable release of osTicket to your local machine.Extract the downloaded osTicket archive to your desired installation directory on your server or hosting environment.</p>
<br />

<p>
<img src="https://i.imgur.com/sG8gNFc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Ensure that your server meets the necessary requirements, including a compatible web server (e.g., Apache or Nginx) and the required version of PHP. Adjust server settings as needed.Create a new database for osTicket and a dedicated user with appropriate permissions.</p> 

<p>Note down the database name, username, and password for use during the installation.Configure your web server to serve osTicket files. Create a virtual host or update server block configurations based on your web server (Apache or Nginx).Adjust file permissions to ensure that the web server has the necessary read and write access to osTicket directories. Refer to the osTicket documentation for recommended permissions.</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open a web browser and navigate to the URL where osTicket is installed. The installer will guide you through the initial setup process.Provide the necessary database information during installation, including the hostname, database name, username, and password created in the earlier steps.Configure email settings in osTicket to enable ticket notifications.</p>
  
<p>Specify SMTP settings or use alternative methods based on your email server setup.Complete the installation by creating an administrator account. This account will be used to access the osTicket admin panel, where you can further customize settings and manage support tickets.</p>
<br />
