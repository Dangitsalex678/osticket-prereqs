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
<img src="https://i.imgur.com/iQDp71l.png" height="80%" width="80%" alt="Installing MySQL"/>
</p>
<p>
<b>- Install <a href="https://drive.google.com/file/d/1X7fZtEyxvQAVMWEAAvkV55vSyJFloj5M/view?usp=share_link">MySQL
</p>- When prompted for an install, select "Typical"
</p>- Launch the wizard after install
</p>- When promtped for what configuration, select "Standard Configuration"
</p>- Create a root password and continue the install</b>
</p>
<br />

<p>
<img src="https://i.imgur.com/iQDp71l.png" height="80%" width="80%" alt="Registering PHP"/>
</p>
<p>
<b>- Click the start button and type "IIS"
</p>- Right click "Internet Information Services" and select "Run as Administrator"
</p>- Select "PHP Manager" from the menu
</p>- Select "Register new PHP Menu"
</p>- Locate and select the "php-cgi" application in the PHP folder
</p>- Restart the server by clicking on the server's name in the left menu under "Connections", Then press "Restart" on the right menu under "Manage Server"</b>
</p>
<br />

<p>
<img src="https://i.imgur.com/3purGNE.png" height="80%" width="80%" alt="Installing osTicket"/>
</p>
<p>
<b>- Install <a href="https://drive.google.com/file/d/1HC9GL8seRoAJ2Ky1gW3N8hQZahvpcqNJ/view?usp=sharing">osTicket
</p>- Extract the zip file
</p>- Rename the "upload" folder to "osTicket"
</p>- Copy the "osTicket" file into C:\inetpub\wwwroot
</p>- Restart the server from IIS Manager</b>
</p>
<br />

<p>
<img src="https://i.imgur.com/Ap2CHCS.png" height="80%" width="80%" alt="Checking osTicket"/>
</p>
<p>
<b>- From the IIS Manager, navigate down the connections menu of the server to Default Web Sites "osTicket"
</p>- Click "Browse *:80(http)" in the right side menu
</p>- osTicket shoud load if everything was set up correctly</b>
</p>
<br />

<p>
<img src="https://i.imgur.com/nb3sunj.png" height="80%" width="80%" alt="Enabling Extensions"/>
</p>
<p>
<b>- From the IIS Manager, navigate down the connections menu of the server back down to Default Web Sites "osTicket"
</p>- Select "PHP Manaager"
</p>- Select "Enable or disable an extension" at the bottom of the page
</p>- Enable "php_imap.dll"
</p>- Enable "php_intl.dll"
</p>- Enable "php_opcache.dll"
</p>- Refresh the osTicket page</b>
</p>
<br />

<p>
<img src="https://i.imgur.com/tRvNX6r.png" height="80%" width="80%" alt="Enabling More Extensions"/>
</p>
<p>
<b>- Rename "ost-sampleconfig.php" to "ost-config.php"
</p>- Right click the file and select properties
</p>- Select "Security" and select "Advanced"
</p>- Cick on "Disable inheritance"
</p>- Select "Remove all inherited permissions from this object"
</p>- Click on "Add" and Click on "Select a Principal"
</p>- Type "Everyone" for the "Object name"
</p>- Select "Full Control" for the permissions and click OK and Apply</b>
</p>
<br />

<p>
<img src="https://i.imgur.com/LDGlMmw.png" height="80%" width="80%" alt="Installing HeidiSQL"/>
</p>
<p>
<b>- Install <a href="https://www.heidisql.com/installers/HeidiSQL_12.3.0.6589_Setup.exe">HeidiSQL
</p>- Follow the instructions of the setup wizard to complete the installation
</p>- Open HeidiSQL
</p>- Select "New" on the bottom left corner
</p>- Enter the Username and Password for MySQL from earlier and select "Open"
</p>- Right click the "Unnamed" database to the left and select "Create new Database"
</p>- Name the new Database "osTicket"
</p>
<br />

<p>
<img src="https://i.imgur.com/Nq1lRq3.png" height="80%" width="80%" alt="osTicket Setup"/>
</p>
<p>
<b>- Go back to IIS and navigate back to the osTicket Site Link
</p>- Click "Continue" and fill out the information for the User and the Admin
</p>- Enter in the MySQL Username and Password in the "Database Settings"
</p>- Enter "osTicket" for the MySQL Database
</p>- Select "Install Now" when finished
</p>- Type "Everyone" for the "Object name"
</p>- Select "Full Control" for the permissions and click OK and Apply</b>
</p>
<br />

<p>
<img src="https://i.imgur.com/qYeETOa.png" height="80%" width="80%" alt="Cleaning Up Files"/>
</p>
<p>
<b>- Delete C:\inetpub\wwwroot\osTicket\setup</b>
</p>
<br />

<p>
<img src="https://i.imgur.com/6Gfa9et.png" height="80%" width="80%" alt="Changing Permissions"/>
</p>
<p>
<b>- Set permissions for "ost-config.php to "Read and Execute"</b>
</p>
<br />
