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

- Azure Virtual Machine with Windows OS
- osTicket Installation Files
- Heidi SQL

<h2>Installation Steps</h2>

<p>
</p>
<p>

Welcome to our tutorial on the prerequisites and installing osTicket. osTicket is an open-source ticketing system that we will later use to create "tickets" and escalate them, as well as make SLA plans, but for now, we must first install osTicket and ensure that it runs properly. First and foremost, create an Azure Virtual Machine that runs a Windows 10 OS and that has 4 CPUs. Make sure to write down the username and password that you have for both and once created, connect to your VM with your public IP address via Remote Desktop (if using Mac, you will have to download Microsoft Remote Desktop from the app store).

<img src="https://i.imgur.com/ab30gGn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/7Fs3Qbc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

Once you have done this, enable IIS (Internet Information Services) and make sure to enable CGI and common HTTP Features, as well as the IIS management console.

<img src="https://i.imgur.com/MnwZVnU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/VdWDvnG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/en1lMN6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


</p>
<br />

<p>
</p>
<p>
  
We will now need to install the PHP manager for IIS, using the installation files that are linked here. https://drive.google.com/drive/u/1/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6. After doing this go back to the installation files and install the re-write module, then create a new folder within the C drive, name this folder C:\PHP. After you have done this, go back to the installation files and download PHP 7.3.8 and unzip all the contents into C:\PHP

<img src="https://i.imgur.com/USS8nz2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/yo8WKCw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/QTNaTWd.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/zFrCn8v.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/f22EsAl.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

</p>
<br />

<p>
</p>
<p>

Go back to your installation files and now install Microsoft Visual C++ and MySQL. After installing MySQL, select the standard configuration, launch the configuration wizard, and create your account. Make sure to write down your username and password to remember it when you log back in.

<img src="https://i.imgur.com/TrCu9zv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/Kk8xr7e.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/tqxTADu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/jjZ1NXb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


</p>
<br />



<p>
</p>
<p>

After you have done this, open up IIS again as an admin and register PHP from within IIS. We can now install osTicket v1.15.8. Go back to the installation files folder and download it from there. After this, extract and copy the "upload" folder to c:\inetpub\wwwroot.

<img src="https://i.imgur.com/JhIv248.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/cX2z6ct.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/5qrajdt.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


</p>
<br />


<p>
</p>
<p>
After you have done this, open up IIS again as an admin and register PHP from within IIS. We can now install osTicket v1.15.8. Go back to the installation files folder and download it from there. After this, extract and copy the "upload" folder to c:\inetpub\wwwroot.
</p>
<br />
