# Setting up Ubuntu Linux on a Virtual Machine (using Mac OS)

<h2> Virtual Machines </h2>

<br>A virtual machine is a safe (and easy to remove) option for trying out a new operating system. Virtual machines allow us to use a portion of our computer's resources to run a totally separate 'simulated computer' or <em>virtual machine</em>.
This virtual machine can even use a totally different operating system!  For example, I could be using a Windows computer, and then run a simulated Linux virtual machine and be able use both at the same time!    

Go to https://virtualbox.org/ and download the newest version of their VirtualBox software (as of this writing is version 6.1)

[![image](https://user-images.githubusercontent.com/12129459/123864712-12468580-d8f9-11eb-990f-c05538c4fcfa.png)](https://www.virtualbox.org/wiki/Downloads)

There should be a large blue 'Download' button in the center of your browser window.  

![image](https://user-images.githubusercontent.com/12129459/124480235-0d5c5880-dd75-11eb-8b21-fc5cc2e4f515.png)

When you click on that 'Download' button, it will take you to their <a href="https://www.virtualbox.org/wiki/Downloads"> downloads page </a> where you have to select your <em>CURRENT</em> operating system. In this example, I am using a Mac computer, so I will click on the "OS X hosts" option.  This is because Mac (OS X) will be the _host_ for our new virtual machine. 

Click on the appropriate link that matches your current operating system.  

That should start a download of the Virtualbox installer.

 <hr>
 
<h2> Installing Virtualbox</h2>

![image](https://user-images.githubusercontent.com/12129459/124480859-b1460400-dd75-11eb-844a-47f4d877cca5.png)

Find that VirtualBox installer that you just downloaded.  In my case, the file was in my _Downloads_ folder under the name **VirtualBox-6.1.22-144080-OSX.dmg** but it may have a slightly different file name for you depending on what version you downloaded. 

![image](https://user-images.githubusercontent.com/12129459/124481026-d9356780-dd75-11eb-8db5-26084884936e.png)

Double click on that VirtualBox installer to start the installation process.

![image](https://user-images.githubusercontent.com/12129459/124507240-66d77e00-dd9b-11eb-8765-67328f538c99.png)

The first thing that will happen is that your mac will panic that you are trying to install software from the outside world. 

Click **Continue** on that pop-up message. 
<hr>

![image](https://user-images.githubusercontent.com/12129459/124508128-4b6d7280-dd9d-11eb-97d2-f10c1b51fe2d.png)

Click **Continue** on that first page of the installer. 
<hr>

![image](https://user-images.githubusercontent.com/12129459/124508184-617b3300-dd9d-11eb-8afa-abdedabe2da8.png)

Continue through the installation using the defaults at each step. Click **Install** on this screen. 
<hr>

![image](https://user-images.githubusercontent.com/12129459/124508937-e31f9080-dd9e-11eb-91f9-de53f2822e06.png)

At least once during this installation, you will be asked to provide a username and password in order to continue. Enter the user name and password that will allow you to make installations on your device, and click **Install Software**.
<hr>


![image](https://user-images.githubusercontent.com/12129459/124509478-0dbe1900-dda0-11eb-95df-b3d50e543b48.png)


The next error message that may pop-up will _seem_ to break the entire installation.  Don't worry, it's fine. 
<hr>

![image](https://user-images.githubusercontent.com/12129459/124509173-78228980-dd9f-11eb-8617-0fa2b77e320f.png)

You might get an error that says "System Extension Blocked".  
Click on "Open Security Settings"
<hr>

![image](https://user-images.githubusercontent.com/12129459/124509758-71e0dd00-dda0-11eb-9082-8edc4cc53352.png)
In the computer's Security and Privacy settings, you should have an "Allow" button that will you can click to enable programs by Oracle (such as VirtualBox) to run. 
Click the **Allow** button.
<hr>

![image](https://user-images.githubusercontent.com/12129459/124509877-ace31080-dda0-11eb-9d68-bca84a7a3360.png)
The program should now be installed.  But if you want to be sure, you can run the installer program again, this time it should work and give you a green checkmark of success at the end.  

Installation is complete for our VirtualBox. Next we need a download of the Linux Operating system, and to put those two things together.  Read on. 
<hr>



<h2> Downloading a Linux Desktop image (.iso)</h2>

Linux has countless varieties (called 'distributions' or 'distros'), each one can be tailor made for a specific purpose or style.  Being free and open-source, anyone willing to put in enough time and effort could create their own personal Linux distribution at anytime. 


For this beginner course, we will be using a user friendly Linux distribution called _Ubuntu_.  We specifically want _Ubuntu version 20.04.2.0 LTS_ (the LTS stands for 'long term support'). 


You can find a download link for this version at the <a href="https://ubuntu.com/download/desktop"> downloads page </a> of Ubuntu's official website. (https://ubuntu.com/download/desktop)

This is going to be a LONG download (~3 Gigs of space).

<hr>

<h2> Setting up your new Linux Virtual Machine</h2>

![image](https://user-images.githubusercontent.com/12129459/124511277-bf127e00-dda3-11eb-8beb-0a5d2272dfa2.png)

If the installation was successful, you should see a VirtualBox icon in your Applications folder.  Double click on that new VirtualBox icon. 

![image](https://user-images.githubusercontent.com/12129459/124483869-cff9ca00-dd78-11eb-9da5-699882e29f92.png)

In your VirtualBox software, click the **New** button.  

<hr>

![image](https://user-images.githubusercontent.com/12129459/124484005-f455a680-dd78-11eb-89d5-8cf8783fb280.png)

Give your virtual machine a name. - I called mine UbuntuVM, but you can call yours whatever you want.  

In the dropdown menu for _Type:_  select **Linux**

In the _Version_ dropdown, select **Ubuntu (64-bit)**.

Click **Continue**. 

<hr>

![image](https://user-images.githubusercontent.com/12129459/124510499-f3853a80-dda1-11eb-813d-724a48d3587b.png)

On the next page, it will ask you how much Memory (RAM) you want to allocate to the virtual machine. 
_**As a rule of thumb, choose one quarter of the available ram.**_  In this case, I have ~32000 MB (or 32 GB) of RAM, so I will chose 1/4 of that, and select around 8000 MB (8 GB).  The absolute numbers for you may be different, but moving the slider to be 1/4 the way up is a safe starting point.  When you do not have the virtual machine running, your default operating system will have access to 100% of the RAM again. 

Click **Continue**. 

<hr>

![image](https://user-images.githubusercontent.com/12129459/124510596-2cbdaa80-dda2-11eb-8eba-d528a3aa97f5.png)

On the Hard disk page, select **Create a Virtual hard disk now**

Click **Create**. 

<hr>

![image](https://user-images.githubusercontent.com/12129459/124510616-39da9980-dda2-11eb-8045-784373924cfc.png)

On the Hard disk file type page, pick **VDI (VirtualBox Disk)** . 

Click **Continue**. 

<hr>

![image](https://user-images.githubusercontent.com/12129459/124510639-44952e80-dda2-11eb-9305-bc1d65765bb4.png)

On the next screen, about storage, select **Dynamically allocated**. 

Click **Continue**. 

<hr>

![image](https://user-images.githubusercontent.com/12129459/124510658-4ced6980-dda2-11eb-897c-c21e62b8c31d.png)

Lastly, I used the default 10 GB of hard drive space.  My computer has 50 GB free, so that shouldn't be a problem, but you may need to clear up some space.  Note, since I chose "dynamically allocate" in the previous step, this virtual machine can take UP TO 10 GB.  It isn't already taking up that much space.  

Click **Create**. 

<hr>

Now, we find ourselves back on the main screen for our VirtualBox program.  

We should now have one new virtual machine listed on the left side. Note: It never asked us for our Ubuntu iso file. It will ask for that the first time we start that virtual machine.  

![image](https://user-images.githubusercontent.com/12129459/124510743-81612580-dda2-11eb-8fff-e7ebdb7c2890.png)

With your new virtual device selected, click the **Start** button.

<hr>

![image](https://user-images.githubusercontent.com/12129459/124511923-34328300-dda5-11eb-908d-bf7d1654fe61.png)
The first error message will be a warning about accessibility features.  We will want to say yes, so that our keyboard and mouse can interact with our new virtual machine.  

Click **Open System Preferences**
<hr>

![image](https://user-images.githubusercontent.com/12129459/124512061-85427700-dda5-11eb-898d-78320fbb9420.png)

We are back in the Security & Privacy settings again.  This time we are in the 'Privacy' tab. 
We can see a greyed out section in the middle that has an empty checkbox beside "VirtualBox".  


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

When you eventually go to either to shutdown this virtual machine, or close the VirtualBox program that it lives within, you will be given 3 choices.  My suggestion is to go with the default **Send the shutdown signal**.

<hr>

![image](https://user-images.githubusercontent.com/12129459/123859855-2be4ce80-d8f3-11eb-9314-bebe8625eacc.png)

When you want to start up your Linux virtual machine again, you can open up your VirtualBox software.

![image](https://user-images.githubusercontent.com/12129459/123843340-d0f5ac00-d8df-11eb-8150-a93ab92d7b6d.png)

Select that same Ubuntu virtual machine from the list, and press the green **Start** button. All of those pesky setup steps only needed to be done once.    
