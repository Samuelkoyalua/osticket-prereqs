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
