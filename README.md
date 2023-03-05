# <p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com/watch?v=K7T_JjvEamg)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- We will Create a Virtual Machine through Azure
- I will install/Enable IIS in windows with CGI
- I will download and install PHP Manager for IIS
- Install the Rewrite Module
- Make sure the directory C:\PHP is created. 
- Download your PHP 7.3.8
- Install your VC redit.x86.exe
- Lastely download and install MYSQL 5.5.62

<h2>Installation Steps</h2>

<p>
<img src=<a href="<a href="https://imgur.com/0sMhwlJ"><img src="https://i.imgur.com/0sMhwlJ.png" title="source: imgur.com" /></a>
</p>
<p>
We will follow the steps and create a WIndows 10 virtual Machines(VM) on Azure software. We can complete theses by opening Virtaul Machine = Create = Windsows or Mac, then we will create a username and password = Review and lastely create.
</p>
<br />

<p>
<img src=" href="https://imgur.com/HMTrfjp"><img src="https://i.imgur.com/HMTrfjp.png" title="source: imgur.com" /></a>
</p>
<img src=<a  href="
                                                                                                 
The second step would be setting up a Remote Desktop Connection, This process would connect our virtual machines by using the assigned IP address when we created our Virtual machine in Azure. Use the correct credentials you created to sign into your virtual machine to keep everything organized.
</p>
<br />

<p>
<img src=<a href=<a href="https://imgur.com/DCoZGWl"><img src="https://i.imgur.com/DCoZGWl.png" title="source: imgur.com" /></a>
<img src=<a href="https://imgur.com/xwmzmUX"><img src="https://i.imgur.com/xwmzmUX.png" title="source: imgur.com" /></a>
</p>
<p>
We have different ways to get to the Control Panel. We can either go straight to the start menu and then serach for the control panel then click on it or Right-click on your windows menu = Run = Control.
  
</p>
<img src=
<img src=<a href="https://imgur.com/MeYMfzT"><img src="https://i.imgur.com/MeYMfzT.png" title="source: imgur.com" /></a>
<br />
After opening the control Panel we will navigate to the program and feature under that we will click  on Turn Windows features on or off> Internet information Service > World Wide Web service > Application Development features then > CGI.
<img src="<a href="https://imgur.com/eBXCfuf"><img src="https://i.imgur.com/eBXCfuf.png" title="source: imgur.com" /></a>While Activating CGI this will allows us to host the webpage above on my Vrtual Machine.We will test this by typing 127.0.0.1 into google on My VM. The result will load in the above picture.
                                                                                                        <img src=<a href="https://imgur.com/Yp66Sqp"><img src="https://i.imgur.com/Yp66Sqp.png" title="source: imgur.com" /></a>
- Our next step is downloading VC_Redlist Software, This is needed for our PHP to work.                  - Download and Install your MSQL Server.
   This server is were our osTicket will be opreating from, The username used to set up the SQL would be root and password: password1
