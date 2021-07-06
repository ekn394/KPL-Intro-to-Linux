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

[![image](https://user-images.githubusercontent.com/12129459/124644449-4a514980-de60-11eb-83f7-c9fe4b2cc260.png)](https://ubuntu.com/download/desktop)

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

![image](https://user-images.githubusercontent.com/12129459/124513053-e5d2b380-dda7-11eb-9a7b-307cbbb15fb8.png)

Click on the padlock in the bottom left corner to be able to make changes. 

<hr>


![image](https://user-images.githubusercontent.com/12129459/124513114-0e5aad80-dda8-11eb-8b20-0e78e063240e.png)

Once again, we will need to supply an administrator User Name and Password, then click the **Unlock** button.
<hr>

![image](https://user-images.githubusercontent.com/12129459/124513177-35b17a80-dda8-11eb-88da-a9a3df662195.png)

With that unlocked, we chould be able to **click on the checkbox beside VirtualBox.** 

You may want to click the lock again to lock in these settings. 

<hr>

![image](https://user-images.githubusercontent.com/12129459/124513308-7f01ca00-dda8-11eb-9004-b3b8befaaf6c.png)

On this first start-up for this virtual machine, it will now ask for the location of your chosen operating system iso file.   

**Click the folder icon**   ![image](https://user-images.githubusercontent.com/12129459/123845032-b91f2780-d8e1-11eb-9d63-bdcdffedb326.png)

If you don't have any 'disk images' loaded here (I don't either), then you will need to click the **Add button** and locate that Ubuntu iso file. 

![image](https://user-images.githubusercontent.com/12129459/124513408-c2f4cf00-dda8-11eb-8de6-16ec2236d51a.png)

Then click **Add**

![image](https://user-images.githubusercontent.com/12129459/124513454-d9028f80-dda8-11eb-8a05-0076e3132591.png)

Locate the Ubuntu iso file that we downloaded earlier, and click **Open**. 

![image](https://user-images.githubusercontent.com/12129459/124513490-f20b4080-dda8-11eb-9824-4a33c982a065.png)

Now with your Ubuntu file selected, you can click the **Choose** button. 

<hr>

![image](https://user-images.githubusercontent.com/12129459/124513535-02232000-dda9-11eb-91d3-da6c5380d3a4.png)

Finally, click **Start**

<hr>

<h3> First Boot Up into Ubuntu Linux</h3>

![image](https://user-images.githubusercontent.com/12129459/124513580-18c97700-dda9-11eb-8926-8c6acf1af2ca.png)

You might get some mini-pop up messages letting you know that they keyboard and mouse can interact with this device, sure.  Close those popups. 

<hr>

![image](https://user-images.githubusercontent.com/12129459/124513740-7958b400-dda9-11eb-9f93-5a09aad5dbdc.png)

After a few seconds I get an screen that asks me if I want to Try or Install Ubuntu.  I want to **Install Ubuntu**.

![image](https://user-images.githubusercontent.com/12129459/124513801-9a210980-dda9-11eb-8e52-54e42c594e29.png)

For Keyboard layout.  I choose the default, **English (US)**, selected **Continue**.  
<hr>

![image](https://user-images.githubusercontent.com/12129459/124513910-d3f21000-dda9-11eb-8f74-58b4859e962c.png)

Leave all of the default options as they are and click **Continue**.
<hr>

![image](https://user-images.githubusercontent.com/12129459/124513950-eec48480-dda9-11eb-9152-979482beb781.png)

This screen can look scary because it asks if you want to "Erase disk and install Ubuntu".  Yes.  We want to erase the Virtual machine, and install Ubuntu.  Leave the defaults just as they are and click **Install Now**.  
<hr>

![image](https://user-images.githubusercontent.com/12129459/124514053-26cbc780-ddaa-11eb-8698-77e82c566bf8.png)

This message tells you which partitions (of your virtual machine) will be changed to Linux.  Again, don't stress out about any of this, just click **Continue**.
<hr>

![image](https://user-images.githubusercontent.com/12129459/124514112-4fec5800-ddaa-11eb-8abb-b85479eabbe5.png)

You can select your default location/timezone.  It predicts that "Toronto" is a good location for me, and I will just leave it as is and click **Continue**.
<hr>

![image](https://user-images.githubusercontent.com/12129459/124514201-790ce880-ddaa-11eb-998e-b54044432937.png)

Almost there, don't give up.  

At this point you can give a username and create a password that you will use to log in to your new Linux virtual machine.  **Don't forget this password, you will need it later!**

Click **Continue**

<hr>

![image](https://user-images.githubusercontent.com/12129459/124514310-c1c4a180-ddaa-11eb-902b-681286f851a0.png)

Sit back and wait for a few minutes while Ubuntu goes through the first time setup proccess.  It doesn't hurt to read the promotional material scrolling by about what comes with your brand new Ubuntu installation. 

<hr>

![image](https://user-images.githubusercontent.com/12129459/124514534-42839d80-ddab-11eb-8150-1afca694412c.png)

When the installation is complete, it will say that you need to restart the computer.  You only need to restart the _virtual machine_, not your regular computer.  

Press the **Restart Now** button.  

<hr>

![image](https://user-images.githubusercontent.com/12129459/124514600-67781080-ddab-11eb-83c4-c08a810cbd41.png)

This first time restart will get stuck at a step that says "Please remove the installation medium, then press ENTER:".  The virtual machine *THINKS* that we have some kind of Ubuntu installation USB stick plugged in (we don't, but that is how it thinks it was setup).  It's fine.  

Just **press the return key on your keyboard**.  This is all just first time setup stuff that shouldn't ever come up again.
The onscreen keyboard say press ENTER.  If you are using a Mac keyboard, that is the _return_ key. 

<br>

![image](https://user-images.githubusercontent.com/12129459/124516523-d6576880-ddaf-11eb-8c0a-82dd9a5ed71d.png)

Click on your chosen username, and type in your chosen password and press the **return** key. 

<hr>

![image](https://user-images.githubusercontent.com/12129459/123857242-0dc99f00-d8f0-11eb-832b-baa7261585c8.png)

The first screen that you are greeted with, similar to Windows computers, is a bunch of nonsense that you don't need.  

Click **Skip**, then **Next**, then I chose "No, don't send system info", **Next**, I left the location services off (which was the default). And then finally, **Done**.  

<hr>

![image](https://user-images.githubusercontent.com/12129459/124516630-220a1200-ddb0-11eb-8e76-b4b3d29f1943.png)

**Congratuations, you now have a virtual Ubuntu Linux computer!**

<hr>

![image](https://user-images.githubusercontent.com/12129459/124516760-6d242500-ddb0-11eb-9f03-dedced8bc566.png)

One last Mac keyboard related item to address. 

Notice that in the bottom right corner of this virtual machine, it will probably have a down arrow, then Left, then the Command symbol.  ![image](https://user-images.githubusercontent.com/12129459/124517439-f6882700-ddb1-11eb-851b-a0df7a844f6a.png)

The VirtualBox program had to choose some key (which they call the 'host key') as a way to switch between having your keyboard communicating with the virtual machine, or to the host computer.  On a Mac it VirtualBox chooses the left Command key, which I think is a poor choice.  The Command key on a mac keyboard takes on the same role as the "Windows" key on a Windows computer.  This key is very useful on Ubuntu Linux as the 'search' key that we will use (frequently) in this course.  I suggest you change the "host key" to be something other than the Left Command key.  I will show how to change it to the ... Right Command key.   

<hr>

![image](https://user-images.githubusercontent.com/12129459/124517292-9b563480-ddb1-11eb-8d19-0711335c2392.png)

Right-click on that down arrow icon and select **Keyboard Settings...**

<hr>

![image](https://user-images.githubusercontent.com/12129459/124517380-d2c4e100-ddb1-11eb-82b6-e1f54d55e629.png)

Where you see Left Command, click there.  Then press the right-side Command key, on your keyboard. 

![image](https://user-images.githubusercontent.com/12129459/124517466-099af700-ddb2-11eb-9ec7-5f31c73bfe25.png)

This is trickier than it seems, but there is an eraser tool if you accidentally assign the wrong key.  
It should look like the image above, where the shortcut is no longer Left-Command.  (You don't _have_ to use Right-Command, but it would be convenient for you to change this away from being Left-Command.  

Click **OK** and everything should be good to go. 

<hr>

![image](https://user-images.githubusercontent.com/12129459/124517634-71514200-ddb2-11eb-8e61-35740b955278.png)

To test out that search key, press the left-side Command key, and Linux _should_ bring up a search field. 

This last step isn't absolutely critical, but I think it will be helpful to have the search key on your keyboard working.  

This time, for sure, we are done our initial setup! Congratulations!

<hr>

![image](https://user-images.githubusercontent.com/12129459/124517771-d147e880-ddb2-11eb-859e-6d6d5abda77e.png)

When you eventually go to either to shutdown this virtual machine, or close the VirtualBox program that it lives within, you will be given 3 choices.  My suggestion is to go with **Send the shutdown signal**.  This simulates the steps of you clicking "shutdown". In an emergency, you can select Power off the machine.  That is a bit more abrupt and simulates you holding the power button to kill the power.  Just like in real life, best practice would be to shut down the machine properly so that it can close all of the programs running in the background in the correct order to make sure everything is in good working order.  

<hr>

![image](https://user-images.githubusercontent.com/12129459/124511277-bf127e00-dda3-11eb-8beb-0a5d2272dfa2.png)

When you want to start up your Linux virtual machine again, you can open up your VirtualBox software which can be found in your Applications folder. 

Select that same Ubuntu virtual machine from the list (if you followed these instructions you might have named it 'UbuntuVM', and press the green **Start** button. All of those pesky setup steps only needed to be done once.    

