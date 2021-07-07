# Setting up Ubuntu Linux on a Virtual Machine (using Windows)

<h2> Virtual Machines </h2>

<br>A virtual machine is a safe (and easy to remove) option for trying out a new operating system. Virtual machines allow us to use a portion of our computer's resources to run a totally separate 'simulated computer' or <em>virtual machine</em>.
This virtual machine can even use a totally different operating system!  For example, I could be using a Windows computer, and then run a simulated Linux virtual machine and be able use both at the same time!    

Go to https://virtualbox.org/ and download the newest version of their VirtualBox software (as of this writing is version 6.1)

[![image](https://user-images.githubusercontent.com/12129459/123864712-12468580-d8f9-11eb-990f-c05538c4fcfa.png)](https://www.virtualbox.org/wiki/Downloads)

There should be a large blue 'Download' button in the center of your browser window.  

![image](https://user-images.githubusercontent.com/12129459/123864239-86ccf480-d8f8-11eb-95b1-c4f758ec2378.png)

When you click on that 'Download' button, it will take you to their <a href="https://www.virtualbox.org/wiki/Downloads"> downloads page </a> where you have to select your <em>CURRENT</em> operating system. In my case, I am using a Windows computer, so I will click on the "Windows hosts" option.  This is because Windows will be the _host_ for our new virtual machine. 

Click on the appropriate link that matches your current operating system.  

That should start a download of the Virtualbox installer.

 <hr>
 
<h2> Installing Virtualbox</h2>

Find that VirtualBox installer that you just downloaded, and double click on it. In my case, the file was in my _Downloads_ folder under the name **VirtualBox-6.1.22-144080-Win.exe** but it may have a slightly different file name for you depending on what version you downloaded. 

![image](https://user-images.githubusercontent.com/12129459/123866890-a31e6080-d8fb-11eb-9346-0700ff54b077.png)


Click **Next** to begin.

Click **Next** to use the default install location.

It is up to you, but I unchecked the box for Quick Launch Bar, then clicked **Next**. 

Click **Yes**. 

Click **Next**.

Click **Finish**.

<hr>

<h2> Downloading a Linux Desktop image (.iso)</h2>

Linux has countless varieties (called 'distributions' or 'distros'), each one can be tailor made for a specific purpose or style.  Being free and open-source, anyone willing to put in enough time and effort could create their own personal Linux distribution at anytime. 


For this beginner course, we will be using a user friendly Linux distribution called _Ubuntu_.  We specifically want _Ubuntu version 20.04.2.0 LTS_ (the LTS stands for 'long term support'). 

[![image](https://user-images.githubusercontent.com/12129459/124644449-4a514980-de60-11eb-83f7-c9fe4b2cc260.png)](https://ubuntu.com/download/desktop)

You can find a download link for this version at the <a href="https://ubuntu.com/download/desktop"> downloads page </a> of Ubuntu's official website. (https://ubuntu.com/download/desktop)

This is going to be a LONG download (~3 Gigs of space).

<hr>

<h2> Setting up your new Linux Virtual Machine</h2>

In your VirtualBox software, click the **New** button.  

![image](https://user-images.githubusercontent.com/12129459/123841861-13b68480-d8de-11eb-8080-36dbbf752418.png)

<hr>

![image](https://user-images.githubusercontent.com/12129459/123835761-ef0ade80-d8d6-11eb-9524-6850e944bbb8.png)

Give your virtual machine a name. - I called mine UbuntuVM, but you can call yours whatever you want.  

In the dropdown menu for _Type:_  select **Linux**

In the _Version_ dropdown, select **Ubuntu (64-bit)**.

![image](https://user-images.githubusercontent.com/12129459/123842096-63954b80-d8de-11eb-886f-7da9e9403179.png)

Click **Next**. 

<hr>

![image](https://user-images.githubusercontent.com/12129459/123837909-60e42780-d8d9-11eb-83f8-0a6069705d85.png)

On the next page, it will ask you how much Memory (RAM) you want to allocate to the virtual machine. 
_**As a rule of thumb, choose one quarter of the available ram.**_  In my case, I have 8000 MB (or 8 GB) of RAM, so I will chose 1/4 of that, and select around 2000 MB (2 GB).  The absolute numbers for you may be different, but moving the slider to be 1/4 the way up is a safe starting point.  When you do not have the virtual machine running, your default operating system will have access to 100% of the RAM again. 

Click **Next**. 

<hr>

![image](https://user-images.githubusercontent.com/12129459/123838990-9b9a8f80-d8da-11eb-88b8-085494b25da2.png)

On the Hard disk page, select **Create a Virtual hard disk now**

Click **Create**. 

<hr>

![image](https://user-images.githubusercontent.com/12129459/123840809-d0a7e180-d8dc-11eb-8b1d-2e93712cf9ff.png)

On the Hard disk file type page, pick **VDI (VirtualBox Disk)** . 

Click **Next**. 

<hr>

![image](https://user-images.githubusercontent.com/12129459/123841045-15cc1380-d8dd-11eb-89dd-c372be7c6bd8.png)

On the next screen, about storage, select **Dynamically allocated**. 

Click **Next**. 

<hr>

![image](https://user-images.githubusercontent.com/12129459/123842280-993a3480-d8de-11eb-93fa-fd029659a7d5.png)

Lastly, I used the default 10 GB of hard drive space.  My computer has 50 GB free, so that shouldn't be a problem, but you may need to clear up some space.  Note, since I chose "dynamically allocate" in the previous step, this virtual machine can take UP TO 10 GB.  It isn't already taking up that much space.  

Click **Next**. 

<hr>

Now, we find ourselves back on the main screen for our VirtualBox program.  

We should now have one new virtual machine listed on the left side. Note: It never asked us for our Ubuntu iso file. It will ask for that the first time we start that virtual machine.  

![image](https://user-images.githubusercontent.com/12129459/123843340-d0f5ac00-d8df-11eb-8150-a93ab92d7b6d.png)

With your new virtual device selected, click the **Start** button.

<hr>

![image](https://user-images.githubusercontent.com/12129459/123844716-5af24480-d8e1-11eb-87a5-122ba129f82d.png)

On this first start-up for this virtual machine, it will now ask for the location of the operating system iso file.   

**Click the folder icon**   ![image](https://user-images.githubusercontent.com/12129459/123845032-b91f2780-d8e1-11eb-9d63-bdcdffedb326.png)

If you don't have any 'disk images' loaded here (I don't either), then you will need to click the **Add button** and locate that Ubuntu iso file. 

![image](https://user-images.githubusercontent.com/12129459/123845128-d0f6ab80-d8e1-11eb-8bb9-c5f7d3f6b03d.png)

Then click **Add**

![image](https://user-images.githubusercontent.com/12129459/123845389-1e731880-d8e2-11eb-95a9-3489e7983eb7.png)

Locate the Ubuntu iso file that we downloaded earlier, and **double-click on it**. 

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

Use your arrow keys to highlight "Install Ubuntu" and **press the Enter key**. 

<hr>

![image](https://user-images.githubusercontent.com/12129459/123847341-7f9beb80-d8e4-11eb-9237-0ebd3332aea9.png)

This may take a few minutes.

<hr>

![image](https://user-images.githubusercontent.com/12129459/123847885-12d52100-d8e5-11eb-8f3d-5d5cc43194b0.png)

A new (optional) setup window will appear.  I selected **Continue**

Then, I hit **Continue** again to select the default English(US) keyboard layout. 

![image](https://user-images.githubusercontent.com/12129459/123848146-5d569d80-d8e5-11eb-9d70-c390ca12b87d.png)

I also left these as the defaults, and hit **Continue**.
<hr>

![image](https://user-images.githubusercontent.com/12129459/123848286-8e36d280-d8e5-11eb-97e9-070042519b7e.png)

This next page, _looks_ scary.  It is asking if it can erase the disk (hard drive) and install Ubuntu.  _This applies to the Virtual Machine's ...new "Virtual hard drive" not your whole computer!_
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

It asks for some details, I eventually went with the name 'evan' instead of 'me' shown in the screenshot above, but it certainly doesn't need to be your real name.  You also have to chose a (memorable) password.  **Don't forget this password, you will need it!**

Click Continue. 

<hr>

![image](https://user-images.githubusercontent.com/12129459/123855295-bd514200-d8ed-11eb-8674-72db74739274.png)

Sit back and wait for a few minutes while Ubuntu does its first time setup.  It doesn't hurt to read the promotional material scrolling by about what comes with your brand new Ubuntu installation. 

<hr>

![image](https://user-images.githubusercontent.com/12129459/123856075-a7904c80-d8ee-11eb-8459-1f67dca93307.png)

When the installation is complete, it will say that you need to restart the computer.  

Press the **Restart Now** button.  This will only restart the virtual machine, not your regular computer.  

<br>

<hr>

![image](https://user-images.githubusercontent.com/12129459/123993636-99980580-d99a-11eb-8ab9-ccf7dbb98743.png)

It will get stuck at a step that says "Please remove the installation medium, then press ENTER:".  The virtual machine *THINKS* that we have some kind of Ubuntu installation USB stick plugged in (we don't, but that is how it thinks it was setup).  It's fine.  

Just **press Enter**.  This is all just first time setup stuff that shouldn't ever come up again.

<br>

![image](https://user-images.githubusercontent.com/12129459/123856809-867c2b80-d8ef-11eb-8ddd-ad94f065383a.png)

Click on your chosen username.  Type in that password that I mentioned you would need, and press Enter. 

<hr>

![image](https://user-images.githubusercontent.com/12129459/123857242-0dc99f00-d8f0-11eb-832b-baa7261585c8.png)


The first screen that you are greeted with, similar to Windows computers, is a bunch of nonsense that you don't need.  

Click **Skip**, then **Next**, then I chose "No, don't send system info", **Next**, I left the location services off (which was the default). And then finally, **Done**.  

<hr>

![image](https://user-images.githubusercontent.com/12129459/123858120-24242a80-d8f1-11eb-80e2-5cef90d73fef.png)

**Congratuations, setup is complete!**

You now have a virtual computer running Ubuntu Linux 20.04.  

<hr>

![image](https://user-images.githubusercontent.com/12129459/123859369-8d586d80-d8f2-11eb-93fd-dc009d9cbcb3.png)

When you eventually go to either to shutdown this virtual machine, or close the VirtualBox program that it lives within, you will be given 3 choices.  My suggestion is to go with **Send the shutdown signal** buy we will discuss in class different scenarios where you might want to use the other options. 

<hr>

![image](https://user-images.githubusercontent.com/12129459/123859855-2be4ce80-d8f3-11eb-9314-bebe8625eacc.png)

When you want to start up your Linux virtual machine again, you can open up your VirtualBox software.

![image](https://user-images.githubusercontent.com/12129459/123843340-d0f5ac00-d8df-11eb-8150-a93ab92d7b6d.png)

Select that same Ubuntu virtual machine from the list, and press the green **Start** button. All of those pesky setup steps only needed to be done once.    
