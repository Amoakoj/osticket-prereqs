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
   This server is were our osTicket will be opreating from, The username used to set up the SQL would
                                                                                                    be root and password: password1
<img src =<a href="https://imgur.com/GO1buxc"><img src="https://i.imgur.com/GO1buxc.png" title="source: imgur.com" /></a>
We will download and install the MSQL server from our link; This software will be the server on which our osTicket will operate. The name for our osTicket server would be username = root and password:password1 and then we will create a server for our osTicket to use.
<img src= <a href="https://imgur.com/P2QenYi"><img src="https://i.imgur.com/P2QenYi.png" title="source: imgur.com" /></a>
<img src=<a href="https://imgur.com/AV5Erog"><img src="https://i.imgur.com/AV5Erog.png" title="source: imgur.com" /></a>
<img src=<a href="https://imgur.com/7rty0Pr"><img src="https://i.imgur.com/7rty0Pr.png" title="source: imgur.com" /></a>
<img src=<a href="https://imgur.com/JOdfaPp"><img src="https://i.imgur.com/JOdfaPp.png" title="source: imgur.com" /></a>
We will open IIS and set it to admin; Then we will follow these steps open PHP Manager = Register for a new PHP Enter: C>PHP =php-cgi.exe.Now restart our server. 
<img src= <a href="https://imgur.com/4fDrd8d"><img src="https://i.imgur.com/4fDrd8d.png" title="source: imgur.com" /></a>
 Our step would be downloading and installing osTicket software. Open osticket= upload; Then we will Extract the upload file into C:= lnetpub=wwwroot. Now we will rename the "upload" folder to "osTicket." Then we will return to ISS and restart the server.
<img src=<a href="https://imgur.com/2GfI5Nl"><img src="https://i.imgur.com/2GfI5Nl.png" title="source: imgur.com" /></a>
In IIS = Sites = default Web Service = osTicket = Browse *80 to open the osTicket in our internet browser.                                                                                                                
<img src=<a href="https://imgur.com/fstEYSy"><img src="https://i.imgur.com/fstEYSy.png" title="source: imgur.com" /></a>
<img src= <a href="https://imgur.com/vO3mkXr"><img src="https://i.imgur.com/vO3mkXr.png" title="source: imgur.com" /></a>
Now we need to enable some extensions so that our osTicket can operate. In our ISS software, we have to open sites = osTicket = PHP Manager = Enable or disable extensions, enable extensions:ph.pop.cash.dll,phplmap.dll,phpintl.dll. Then we will refresh the osTicket tab in our internet explorer.
<img src=<a href="https://imgur.com/cnl6WfD"><img src="https://i.imgur.com/cnl6WfD.png" title="source: imgur.com" /></a>
Next rename the file "Ostsampleconfig" to "Ostconfig". This file can be found in our Browse = wwwroot = include = Ostsampleconfig.
<img src=<a href="https://imgur.com/UR5JbT9"><img src="https://i.imgur.com/UR5JbT9.png" title="source: imgur.com" /></a>
Right-click "ostconfig = open properties = security = advanced = disable ingeritance = remove all permissions. We can now select "Everyone" and apply.                                                     
<img src=<a href="https://imgur.com/Cd5egeh"><img src="https://i.imgur.com/Cd5egeh.png" title="source: imgur.com" /></a>
<img src=<a href="https://imgur.com/8OPYOIw"><img src="https://i.imgur.com/8OPYOIw.png" title="source: imgur.com" /></a>
Download and install Heidi from our link the step to follow aew Next right-click = create new = database = and name it as osTicket.Open osTicket in our internet browser then fill out the installation deatails and install.
<img src=<a href="https://imgur.com/ss14rqV"><img src="https://i.imgur.com/ss14rqV.png" title="source: imgur.com" /></a>
In the next step we will Delect the folder names "setup" this folder is in our osTicket = setup.
<img src=<a href="https://imgur.com/dAgOcck"><img src="https://i.imgur.com/dAgOcck.png" title="source: imgur.com" /></a>
Right-click "ostconfig = properties = security = advanced = disabled inheritance = modify = read only. Then we select "Everyone" and apply.
<img src=<a href="https://imgur.com/7J24XbJ"><img src="https://i.imgur.com/7J24XbJ.png" title="source: imgur.com" /></a>
<img src=<a href="https://imgur.com/YNwPojY"><img src="https://i.imgur.com/YNwPojY.png" title="source: imgur.com" /></a>
Lastly we will open and log in to our osTicket with the credentials we created when filling out the osTicket installation page.
