<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> 

<h2>List of Prerequisites</h2>

- IIS
- PHP Manager
- VC_redistx86
- MySQL 5.5.62
- Rewrite Module
- Heidi SQL

<h2>Installation Steps</h2>

<h2>Setting Up osTicket on Azure VM</h2>

- Create Virtual Machine in Azure:
- Log in to Azure Portal.
  
- Create a new VM with Windows Server.
<img width="1912" height="528" alt="image" src="https://github.com/user-attachments/assets/b81dd1f0-2570-4a3d-a20e-0c1b448ea05b" />

</p>
<p>

- Connect to your VM using the Remote Desktop with the public IP address form the VM. (for mac user use the "windows app")
  
- login with the same login credentials used to create the VM.
  
<img width="1910" height="831" alt="image" src="https://github.com/user-attachments/assets/3f75dcec-7c85-4cc1-afe8-a16758ce2466" />

2. Download the osTicket-Installation-Files.zip

- Inside your VM download the [osTicket-Installation-Files.zip](https://drive.google.com/uc?export=download&id=1b3RBkXTLNGXbibeMuAynkfzdBC1NnqaD)and unzip it onto your desktop. we will use the files to download osticket.
<img width="1116" height="623" alt="image" src="https://github.com/user-attachments/assets/9bd550ea-ecf9-46bd-a3c6-e694e68e0cb1" />

3. Enable ISS with CGI

- Go to the Control Panel and open the programs applet. Under programs, select "Turn Windows features on or off".


<img width="1114" height="627" alt="image" src="https://github.com/user-attachments/assets/ea38498b-dc3e-464a-9026-d1631c05dde1" />

- enable (internet information services) World Wide Web Services -> Application Development Features -> enable (CGI)


<img width="1102" height="620" alt="image" src="https://github.com/user-attachments/assets/3f915a2b-69e0-41f1-90af-c7d81d62d31c" />

- Test if the changes were applied succesfully, type 127.0.0.1 on your browser and the page below should appear.


<img width="1906" height="1028" alt="image" src="https://github.com/user-attachments/assets/9e45380c-4264-462c-82c7-40981ce39878" />

4. Download and install PHP manager from the osTicket-Installation-Files
- (PHPManagerForIIS_V1.5.0.msi)

<img width="1002" height="440" alt="image" src="https://github.com/user-attachments/assets/16a8b25e-0c69-4001-9db0-6999f0833708" />

5. Download and Install the Rewrite Module

- (rewrite_amd64_en-US.msi) from the osTicket-Installation-Files

<img width="1053" height="419" alt="image" src="https://github.com/user-attachments/assets/f0fd4be3-8c22-4e91-8eb9-3e4d58d50d3e" />

6. Creat a directoy in the C drive 

- Go to file explorer and creat the directory C:\PHP


<img width="912" height="591" alt="image" src="https://github.com/user-attachments/assets/061ec363-53e7-458e-869e-36f125a59376" />

7. From the osTicket-Installation-Files intall(php-7.3.8-nts-Win32-VC15-x86.zip) into C:\PHP

- osTicket-Installation-Files unzip the content into the newly created C:\PHP

<img width="910" height="586" alt="image" src="https://github.com/user-attachments/assets/def91755-c556-4d58-8b62-c8f08fd08994" />

8. Download and Install the (VC_redist.x86.exe) 

- install from the osTicket-Installation-Files

<img width="780" height="588" alt="image" src="https://github.com/user-attachments/assets/74b3e7fe-c744-44b5-811a-961f5e6675c9" />

9. Download and install MySQL 5.5.62 (mysql-5.5.62-win32.msi)

- install from the osTicket-Installation-Files

- select the following configurations;

  ->Typical setup

  ->launch configuration


  ->Standard configuration

  <img width="783" height="590" alt="image" src="https://github.com/user-attachments/assets/ec052a10-8163-41cf-ae74-4526076f9026" />












</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
