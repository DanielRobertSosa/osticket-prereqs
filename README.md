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
  <img width="762" height="579" alt="image" src="https://github.com/user-attachments/assets/337a7f03-aab4-45ed-a0d3-d1ad0d43d0a2" />



- the user for this service is going to (username:root) (password:root) for my sql server


<img width="793" height="601" alt="image" src="https://github.com/user-attachments/assets/a08b7e4b-ef05-4c03-aa97-4e2c9f0745c5" />

10. Launch IIS as an administrator

- Search for IIS in the windows search bar and right click it and select open as administrator


<img width="356" height="155" alt="image" src="https://github.com/user-attachments/assets/8b53d52e-1764-441e-a98a-d30fa0dc9a86" />

11. Register PHP from within lIS
- open the PHP manager
- Register new PHP version


<img width="986" height="675" alt="image" src="https://github.com/user-attachments/assets/5d146c2d-3ab2-4e39-9272-5f59c1a88b1b" />

-browse (...)

- go to your C drive

- PHP folder

- php-cgi


<img width="1133" height="389" alt="image" src="https://github.com/user-attachments/assets/79f4e3bd-ce56-4caa-a0fa-57bffa5def96" />

12. Reload IIS (Open IIS, Stop and Start the server)

 -The restart button can be found on the right side of the window
 
<img width="1414" height="475" alt="image" src="https://github.com/user-attachments/assets/16c723fc-5efe-46ef-a3b6-a1d53cd111af" />

13. Download and install osTicket

-from the osTicket-Installation-Files unzip or extract the (osTicketv1.15.8)

![image](https://github.com/user-attachments/assets/cddae31a-a0f3-47e6-91ab-95726e5302e6)

-after extracting the folder click on the folder and then copy the "upload" folder into "c: linetpub\wwwroot"






- open file explorer
- C drive
- inetpub
- wwwroot


<img width="801" height="493" alt="image" src="https://github.com/user-attachments/assets/79c13075-ed35-40ac-b06e-91378a096293" />

- Within "c: linetpub|wwwroot", Rename "upload" to "osTicket"

<img width="902" height="321" alt="image" src="https://github.com/user-attachments/assets/f022fdd8-2c70-450d-ac93-6299ff40857a" />

14. Reload IIS as admin (Open IIS, Stop and Start the server)

 -The restart button can be found on the right side of the window
 
<img width="1365" height="496" alt="image" src="https://github.com/user-attachments/assets/14170c74-a710-4b7e-a437-2269f4476b45" />

15. Launch osTicket

 -On the left hand side of IIS, Expand on the VM name -> Sites - > Default Website -> osTicket

- click on browse *:80(http)

<img width="1357" height="444" alt="image" src="https://github.com/user-attachments/assets/26728d87-cd5b-4dc9-b7ea-b236e54419cd" />

- This should then lead to your browser opening osTicket.


<img width="869" height="829" alt="image" src="https://github.com/user-attachments/assets/53a084fd-2697-44c6-baf1-7827f2dff534" />

16. Enable extensions

- open IIS, sites -> Default -> osTicket
- Double-click PHP Manager

<img width="1412" height="332" alt="image" src="https://github.com/user-attachments/assets/963f62a4-197e-4974-a04a-fb0a02709679" />

Click “Enable or disable an extension”

- Enable: php_imap.dll
- Enable: php_intl.dll
- Enable: php_opcache.dll

<img width="1215" height="477" alt="image" src="https://github.com/user-attachments/assets/fdcfc955-2aba-4004-9a1d-373ce8e4a881" />

17.Refresh osTicket

- Refresh the osTicket site in your browser, some extensions will now appear active 

<img width="869" height="804" alt="image" src="https://github.com/user-attachments/assets/96054b8e-473a-452a-8cbe-a2b25d4ec1e4" />

18.Change ost-config.ph  


- Rename: ost-config.php

From: C:\inetpub|wwwrootlosTicket\includelost-sampleconfig.php


To: C. linetpubiwwwrootlos Ticketinclude lost-config.php

- rename "ost-sampleconfig.ph" to "ost-config.ph"


<img width="904" height="677" alt="image" src="https://github.com/user-attachments/assets/1edbec4c-04d1-49c4-9c9c-81a35aced2f4" />

22. Change ost-config.ph permissions

- Change ost-config.php permissions by right clicking and selecting

- Properties -> Security -> Advance -> Disable inheritance

- Disable inheritance -> Remove All


<img width="755" height="507" alt="image" src="https://github.com/user-attachments/assets/db98891e-8aa1-48cc-a310-8ea7f816a3de" />

- New Permissions -> Everyone -> All|

go to add-> select principal-> Everyone-> click full access-> apply-> ok

<img width="756" height="520" alt="image" src="https://github.com/user-attachments/assets/8f104579-a8fe-41b5-9d5e-6c4d05293a77" />

23. Continue osTicket installation

- Continue the osTicket installer on your browser by filling the first half of the page.

<img width="914" height="949" alt="image" src="https://github.com/user-attachments/assets/f7a7d6f1-6565-466e-a689-03fd9c011f30" />

24. Download and install Heidi SQL from the osTicket-Installation-Files

<img width="771" height="588" alt="image" src="https://github.com/user-attachments/assets/a059116e-a5ec-445e-8a2f-ed8e45f1c1e1" />


- Open Heidi SQL and create a new session 
- fill in username and password as root

username:root 


password:root 

- then click open

<img width="762" height="578" alt="image" src="https://github.com/user-attachments/assets/9669d950-e08e-4612-8802-2c5a5544f097" />



25. Create new database

- On the left side of the window, right click on "Unnamed" and click create new database and name it "osTicket".

<img width="921" height="432" alt="image" src="https://github.com/user-attachments/assets/48e8c7d5-e840-4280-88d5-91dd375fb0ab" />


26. Finish signing in database settings

- Then go back to your osTicket browser and fill up the missing credentials. It should look something like this.

- install now

<img width="420" height="328" alt="image" src="https://github.com/user-attachments/assets/4a876731-35f0-41e9-a108-faa24c11314c" />



27. Finalize osticket installation


<img width="881" height="729" alt="image" src="https://github.com/user-attachments/assets/8f2451f2-eaef-41b3-8577-3ab6d667d763" />
































