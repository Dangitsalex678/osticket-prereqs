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

- Microsoft Azure Account
- Azure Virtual Machines
- <a href="https://drive.google.com/drive/folders/1UsQgjbyDkJKAs8LiZF3UUasNzymwAZSp?usp=share_link"> Installation Files

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/e2VhepU.png" height="80%" width="80%" alt="Creating a Resource Group in Azure"/>
</p>
<p>
<b>- Log into the Azure portal and search and click "Resource Groups"
</p>- Create a resource group for the OS Ticket Lab</b>
</p>
<br />

<p>
<img src="https://i.imgur.com/C3lHGX8.png" height="80%" width="80%" alt="Creating a Virtual Machine in Azure"/>
</p>
<p>
<b>- Create a Windows 10 Virtual Machine with 2-4 CPUs</b>
</p>
<br />

<p>
<img src="https://i.imgur.com/xQB3Y4m.png" height="80%" width="80%" alt="Remote Desktop Application"/>
</p>
<p>
<b>- Connect to the virtual machine with remote desktop using the IP address. The application I used on my Mac was Microsoft Remote Desktop from the App Store</b>
</p>
<br />

<p>
<img src="https://i.imgur.com/mK7mWeb.png" height="80%" width="80%" alt="Installing and Enable IIS"/>
</p>
<p>
<b>- Install and enable IIS
</p>- Go to "Control Panel"
</p>- Click "Programs"
</p>- Then click "Turn Windows Features on or off" 
</p>- Find "Internet Information Services and check to enable it
</p>- Expand the "World Wide Web" Menu
</p>- Expand the "Application Development Features" Menu
</p>- Click to enable "CGI"</b>
</p>
<br />

<p>
<img src="https://i.imgur.com/Esxl8YV.png" height="80%" width="80%" alt="Checking ISS"/>
</p>
<p>
<b>- Go to the browser and navigate to 127.0.0.1
</p>- If IIS is enabled correctly, the screen above should load</b>
</p>
<br />

<p>
<img src="https://i.imgur.com/SSIGSTz.png" height="80%" width="80%" alt="Downloading PHP Manager"/>
</p>
<p>
<b>- Install <a href="https://drive.google.com/file/d/1O981Q9XLgIkjiQSREgY-r5yPB0QodPGJ/view?usp=sharing">PHP Manager for IIS
</p>- Double click to open it after it downloads</b>
</p>
<br />

<p>
<img src="https://i.imgur.com/SSIGSTz.png" height="80%" width="80%" alt="Install Rewrite Module"/>
</p>
<p>
<b>- Install <a href="https://drive.google.com/file/d/1mYIAQmCy9fkeoVt_2R17fijOJ_e-C8Wj/view?usp=share_link">Rewrite Module
</p>- Double click to open it after it downloads</b>
</p>
<br />

<p>
<img src="https://i.imgur.com/05Fdsqq.png" height="80%" width="80%" alt="Install Rewrite Module"/>
</p>
<p>
<b>- Create the directory C:\PHP
</p>- Naviage to the C Drive in the "This PC" tab
</p>- Create a folder named "PHP"</b>
</p>
<br />

<p>
<img src="https://i.imgur.com/AwtVCo9.png" height="80%" width="80%" alt="Installing PHP 7.3.8"/>
</p>
<p>
<b>- Create the directory C:\PHP
</p>- Download <a href="https://drive.google.com/file/d/1i019FQdWA5WFDqEMhwzEfUZATt9NIkN7/view?usp=share_link">PHP 7.3.8 
</p>- Unzip it into the C:\PHP</b>
</p>
<br />

<p>
<img src="https://i.imgur.com/yQHVTKu.png" height="80%" width="80%" alt="Installing MySQL"/>
</p>
<p>
<b>- Install <a href="https://drive.google.com/file/d/1X7fZtEyxvQAVMWEAAvkV55vSyJFloj5M/view?usp=share_link">MySQL</b>
</p>
<br />
