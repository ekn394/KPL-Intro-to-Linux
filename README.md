# KPL-Intro-to-Linux
Class instructions and starter files for the 4-part series on Intro to Linux

<h3> Virtual Machine </h3>

<br>Virtual machines allow us to use a portion of our computer's resources to run a totally separate 'simulated computer' or <em>virtual machine</em>.
This virtual machine can be a totally different operating system too.  For example, I could be using a Windows computer and then run a simulated Linux virtual machine and be able use both at the same time.  A virtual machine is a safe (easy to remove) option for trying out a new operating system.   

Go to https://virtualbox.org/ and download the newest version.  
<br>There should be a HUGE blue 'download' button in the center of your browser window.  
<br>The downloads button will send you to the downloads page, where you have to select your <em>CURRENT</em> operating system.
 
<h3> Installing Virtualbox</h3>

Open up the installer. 

Click Next to begin.

Click Next to use the default install location.

Up to you but I uncheck the box for Quick Launch Bar, then click Next. 

Click Yes. 

Click Next.

Click Finish.

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

We should now have 1 new virtual machine listed on the left hand side. Note it never asked us for the Ubuntu iso file, it will do that the first time we start that virtual machine.  

![image](https://user-images.githubusercontent.com/12129459/123843340-d0f5ac00-d8df-11eb-8150-a93ab92d7b6d.png)

With your new virtual device selected, click the Start button.

<hr>

![image](https://user-images.githubusercontent.com/12129459/123844716-5af24480-d8e1-11eb-87a5-122ba129f82d.png)

On this first start-up for this virtual machine, it will ask you for the location of the operating system iso file.  Here we want to click the folder icon 

Click the folder icon   ![image](https://user-images.githubusercontent.com/12129459/123845032-b91f2780-d8e1-11eb-9d63-bdcdffedb326.png)

If you don't have any 'disk images' loaded here (I don't either), then you will need to click the **Add button** and locate that Ubuntu iso file. 

![image](https://user-images.githubusercontent.com/12129459/123845128-d0f6ab80-d8e1-11eb-8bb9-c5f7d3f6b03d.png)

Then click **Add**

![image](https://user-images.githubusercontent.com/12129459/123845389-1e731880-d8e2-11eb-95a9-3489e7983eb7.png)

Locate the ubuntu iso file that we downloaded earlier, and double click on it. 

![image](https://user-images.githubusercontent.com/12129459/123845524-482c3f80-d8e2-11eb-96a4-ade49588f786.png)

Now with your Ubuntu file selected, you can click the **Choose** button. 

<hr>

![image](https://user-images.githubusercontent.com/12129459/123845608-64c87780-d8e2-11eb-9db1-17c9681a2715.png)

Finally, click **Start**

<hr>

<h3> First Boot Up into Ubuntu Linux</h3>

**Warning: For the next few steps you will need to use your keyboard, not a mouse**

It might ask you for your language of choice.  I choose the default, English, and hit the Enter key on my keyboard.  

![image](https://user-images.githubusercontent.com/12129459/123846573-8a09b580-d8e3-11eb-985b-7aabf6b7ed0e.png)

Next, pick the third option which is to **Install Ubuntu**

Use your arrow keys to highlight "Install Ubuntu" and press the Enter key. 

<hr>

![image](https://user-images.githubusercontent.com/12129459/123847341-7f9beb80-d8e4-11eb-9237-0ebd3332aea9.png)

This will take a minute

<hr>

![image](https://user-images.githubusercontent.com/12129459/123847885-12d52100-d8e5-11eb-8f3d-5d5cc43194b0.png)
A new (optional) setup window will appear.  I selected **Continue**

Next, I hit Continue to select the default English(US) keyboard layout. 

![image](https://user-images.githubusercontent.com/12129459/123848146-5d569d80-d8e5-11eb-9d70-c390ca12b87d.png)

I also left these as the defaults, and hit **Continue**.
<hr>

![image](https://user-images.githubusercontent.com/12129459/123848286-8e36d280-d8e5-11eb-97e9-070042519b7e.png)

This next page, _looks_ scary.  It is asking if it can erase the disk (hard drive) and install Ubuntu.  **This applies to the Virtual Machine's ...new "Virtual hard drive" not your whole computer!** 
If this WASN'T a virtual machine, this would be a very good double check to make sure you want to erase your computer and install Ubuntu.  In this case we are wiping our ...empty virtual machine, and installing Ubuntu. 

If you have been following along so far, and the very top of this window says something like "UbuntuVM [Running] - Oracle VM VirtualBox" ...

![image](https://user-images.githubusercontent.com/12129459/123852943-e0c6bd80-d8ea-11eb-96a9-ab7a2c086e00.png)

...click the **Install Now** button in the bottom right. 

<hr>

![image](https://user-images.githubusercontent.com/12129459/123853299-4ca92600-d8eb-11eb-9a22-e1e954ccb49f.png)

Next it will give you details about partition tables.  Since this is a virtual machine that we can easily delete later with the click of a button, we don't need to stress out about any of those partition table details. Don't worry about it.  There are other circumstances where you might want to write this information down, but in this virtual machine scenario, it doesn't matter, so we can just click **Continue**.

Click Continue. 

<hr>

![image](https://user-images.githubusercontent.com/12129459/123853883-f8527600-d8eb-11eb-8912-85d08ccd2120.png)

You can select your default location/timezone.  It predicts that "Toronto" is a good location for me, and I will just leave it as is. 

Click Continue. 

<hr>

![image](https://user-images.githubusercontent.com/12129459/123854463-bd9d0d80-d8ec-11eb-9e84-71b885cce7e9.png)

It asks for some details, I chose the name 'evan' but it doesn't need to be your real name, and I chose a memorable password.  **Don't forget this password, you will need it!**

Click Continue. 

<hr>

![image](https://user-images.githubusercontent.com/12129459/123855295-bd514200-d8ed-11eb-8674-72db74739274.png)

Sit back and wait for a minute or two while it sets up for the first time, and it doesn't hurt to read the promotional material scrolling by about what comes with your brand new Ubuntu installation. 




