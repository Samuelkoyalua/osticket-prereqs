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

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Azure Virtual Machine
- Internet Information Services (IIS)
- PHP Manager
- Create the directory C:\PHP
- download and install VC_redist.x86.exe

- Item 5
osTicket prerequisite and installation files https://drive.google.com/drive/u/1/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6

<h2>Installation Steps</h2>

<p>
<img src="https://imgur.com/q63vsjG.png" height="40%" width="40%" alt="Disk Sanitization Steps"/>
</p>
<p>
First start by creating a resource group and use a region of your choice
</p>
<br />

<p>
<img src="https://i.imgur.com/rseqvCk.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

<p>
<img src="https://i.imgur.com/Pt9vp7S.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
After successfully provisioning the resource group, the subsequent step involves deploying a virtual machine (VM). Following this, we'll proceed to access the VM by utilizing its public IP address through Remote Desktop Protocol (RDP).</p>
<br />
<p>
<img src="https://i.imgur.com/u3CkDuV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In this step, we aim to install and activate Internet Information Services (IIS) on Windows, along with CGI and Common HTTP features, as well as World Wide Web Services with Application Development Features enabled.




</p>
<br />

<p>
<img src="https://i.imgur.com/072Z9vi.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Let's acquire and install PHP Manager for IIS (PHPManagerForIIS_V1.5.0.msi) from the installation files provided.


</p>
<br />

<p>
<img src="https://i.imgur.com/RaQBoiT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Next step would be to download and install the rewrite module


<p>
<img src="https://i.imgur.com/itO6xHd.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src="https://i.imgur.com/Q4K8vDF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

Once the PHP file has been successfully downloaded, proceed to navigate to the "Files" directory. Then, right-click on the downloaded PHP file and select the "Extract All" option to initiate the extraction process.






<p>
<img src="https://i.imgur.com/2WtP09m.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>


Now, let's proceed with the acquisition and installation of VC_redist.x86.exe from the provided installation files. This crucial step involves retrieving the necessary redistributable package to ensure seamless compatibility and optimal performance. Once downloaded, we'll meticulously execute the installation process, aligning our system environment with the requisite components for enhanced functionality and reliability.











<p>
<img src="https://i.imgur.com/smuMb0g.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

  
</p>

Next we download and install MySQL 5.5.62








<p>
<img src="https://i.imgur.com/p4TgBGj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

  
</p>


<p>
<img src="https://i.imgur.com/PItcElJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

  
</p>




<p>
<img src="https://i.imgur.com/vrjjqVK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

  
</p>


Access IIS with administrative privileges, proceed to register PHP directly within the IIS interface, and then refresh IIS by stopping and starting the server to implement the changes effectively.







<p>
<img src="https://i.imgur.com/z8AjIf9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

  
</p>


To begin the installation of osTicket v1.15.8, follow these steps:

Download osTicket from the Installation Files Folder.
Extract the downloaded files and locate the "upload" folder.
Copy the entire "upload" folder to the directory "c:\inetpub\wwwroot".
Inside the "c:\inetpub\wwwroot" directory, rename the copied "upload" folder to "osTicket".
Reload IIS by stopping and then starting the server.
Access IIS and navigate to sites -> Default -> osTicket.
On the right-hand side, click on "Browse *:80" to launch osTicket in your browser.






<p>
<img src="https://i.imgur.com/3x8tDlD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

  
</p>



<p>
<img src="https://i.imgur.com/Z1SVDkc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

  
</p>



Navigate to sites -> Default Web Site -> osTicket.
Double-click on PHP Manager to access its settings.
Within PHP Manager, locate the section for enabling or disabling extensions.
Enable the following extensions:
php_imap.dll
php_intl.dll
php_opcache.dll








<p>
<img src="https://i.imgur.com/BRE7fvD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

  
</p>



Let's rename the configuration file "ost-sampleconfig.php" to "ost-config.php". This file is located within the directory "C:\inetpub\wwwroot\osTicket\include". By completing this renaming process, we ensure that osTicket utilizes the correct configuration settings, thus facilitating seamless operation and customization.






<p>
<img src="https://i.imgur.com/184p59Y.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

  
</p>


permission granted to everyone
