# KPL-Intro-to-Linux
Class instructions and starter files for the 4-part series on Intro to Linux

<h3> Virtual Machine </h3>

<br>Virtual machines allow us to use a portion of our computer's resources to run a totally separate 'simulated computer' or <em>virtual machine</em>.
This virtual machine can be a totally different operating system too.  For example, I could be using a Windows computer and then run a simulated Linux virtual machine and be able use both at the same time.  A virtual machine is a safe (easy to remove) option for trying out a new operating system.   

Go to https://virtualbox.org/ and download the newest version.  
<br>There should be a HUGE blue 'download' button in the center of your browser window.  
<br>The downloads button will send you to the downloads page, where you have to select your <em>CURRENT</em> operating system.
 
<h3> Installing Virtualbox</h3>

<br>Open up the installer. 
<br> Click Next to begin.
<br> Click Next to use the default install location.
<br> Up to you but I uncheck the box for Quick Launch Bar, then click Next. 
<br> Click Yes. 
<br> Click Next.
<br> Click Finish

<h3> Downloading a Linux Desktop image (.iso)</h3>
For this course we will want Ubuntu 20.04.2.0 LTS which you can find at the top of this page. 
<br>
https://ubuntu.com/download/desktop
  
<br>There are two options, 20.04.2.0 LTS (meaning Long Term Support)
and another download option, version 21.04. We want the earlier one, 20.04.2.0 LTS. 

This will be a LONG download (~3 Gigs of space)

<h3> Setting up your new Linux Virtual Machine</h3>

In your VirtualBox software, click the **New** button.  

![image](https://user-images.githubusercontent.com/12129459/123841861-13b68480-d8de-11eb-8080-36dbbf752418.png)

<hr>

![image](https://user-images.githubusercontent.com/12129459/123835761-ef0ade80-d8d6-11eb-9524-6850e944bbb8.png)

Give your virtual machine a name. - I called mine UbuntuVM, but you can call yours whatever you want.  

In the dropdown menu for _Type:_  select **Linux**

In the _Version_ dropdown, select **Ubuntu (64-bit)**.

![image](https://user-images.githubusercontent.com/12129459/123842096-63954b80-d8de-11eb-886f-7da9e9403179.png)

Click Next. 

<hr>

![image](https://user-images.githubusercontent.com/12129459/123837909-60e42780-d8d9-11eb-83f8-0a6069705d85.png)

On the next page, it will ask you how much Memory (RAM) you want to allocate to the virtual machine. 
_**As a rule of thumb, choose one quarter of the available ram.**_  In my case, I have 8000 MB (or 8 GB) of RAM, so I will chose 1/4 of that, and select around 2000 MB (2 GB).  The absolute numbers for you may be different, but moving the slider to be 1/4 the way up is a safe starting point.  When you do not have the virtual machine running, your default operating system will have access to 100% of the RAM again. You can choose less than that, but your vitural 

Click Next. 

<hr>

![image](https://user-images.githubusercontent.com/12129459/123838990-9b9a8f80-d8da-11eb-88b8-085494b25da2.png)

On the Hard disk page, select **Create a Virtual hard disk now**

Click Create. 

<hr>

![image](https://user-images.githubusercontent.com/12129459/123840809-d0a7e180-d8dc-11eb-8b1d-2e93712cf9ff.png)

On the Hard disk file type page, pick **VDI (VirtualBox Disk)** . 

Click Next. 

<hr>

![image](https://user-images.githubusercontent.com/12129459/123841045-15cc1380-d8dd-11eb-89dd-c372be7c6bd8.png)

On the next screen, about storage, select **Dynamically allocated**. 

Click Next. 

<hr>

![image](https://user-images.githubusercontent.com/12129459/123842280-993a3480-d8de-11eb-93fa-fd029659a7d5.png)

Lastly, I used the default 10 GB of hard drive space.  My computer has 50 GB free, so that shouldn't be a problem, but you may need to clear up some space.  Note, since I chose "dynamically allocate" in the previous step, this virtual machine can take UP TO 10 GB.  It isn't already taking up that much space.  

Click Next. 

<hr>

Now, we find ourselves back on the main Oracle VM VirtualBox Manager.  

We should now have 1 new virtual machine listed on the left hand side.  Note it never asked us for the Ubuntu iso file, it will do that the first time we start that virtual machine.  

![image](https://user-images.githubusercontent.com/12129459/123843340-d0f5ac00-d8df-11eb-8150-a93ab92d7b6d.png)

With your new UbuntuVM (or whatever you named yours) selected, click the Start button. 


