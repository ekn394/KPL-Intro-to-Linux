# Creating a Bootable USB Flash Drive

<h2> Download Balena Etcher </h2>

Go to https://www.balena.io/etcher/ and click on the green download button. 

![image](https://user-images.githubusercontent.com/12129459/127605761-f133354e-3313-4a5d-83d4-c93c12ccc82b.png)


<hr>

![image](https://user-images.githubusercontent.com/12129459/127606050-235bd26a-45fd-4337-b7f0-701655480da8.png)

Find that installer file in your downloads and run it.  

<hr>

![image](https://user-images.githubusercontent.com/12129459/127606161-d7e02665-3925-4016-8fec-6a7918c392ac.png)

Click on the "I agree" button to install the Etcher software. 

<hr>

![image](https://user-images.githubusercontent.com/12129459/127606389-d78ee11d-fb7e-4bab-832e-5ff1e08c025f.png)

Click on the "Flash from file" button. 

<hr>

![image](https://user-images.githubusercontent.com/12129459/127607079-1cd0c117-4ecd-480f-bffc-7f49b8236465.png)

Select the operating system you want from one of your previously downloaded .iso or .img files.  In this example, I am choosing Ubuntu-20.04.

<hr>

![image](https://user-images.githubusercontent.com/12129459/127607397-a59020a1-e991-4764-b7ad-9a6d5fd2f269.png)

Click Select Target.  

![image](https://user-images.githubusercontent.com/12129459/127607457-61fd7b1c-4ac4-4f3b-a1f7-c98c49d977bc.png)

Click on the checkbox for your USB device.  Then, click on the "Select" button. 

![image](https://user-images.githubusercontent.com/12129459/127607654-452bd0af-7d1a-45dd-885c-f16604b0abaa.png)

Click on the "Flash!" button then sit back and wait for the program to create your bootable usb stick.  

![image](https://user-images.githubusercontent.com/12129459/127607969-b65509fb-cadc-474e-b129-d6bff31877ff.png)

This step may take a few minutes.


## Modifying your BIOS so you can boot from a USB. 
### For Windows 
This will be different for every device and every operating system so it will be difficult/impractical for me to have detailed instructions for every possible version of Windows, for every possible hardware type.  Dell will have a different BIOS screen than a Toshiba which will be different from a Windows Suface, etc.  The BIOS screen will look different on every computer and the menu options are also unique to the manufacturer.   

**Your mission is to get to your computer's BIOS screen.**  

These vague instructions come straight from the Microsoft website. 


_Boot the PC, and press the manufacturer’s key to open the menus. Common keys used: Esc, Delete, F1, F2, F10, F11, or F12._

_Or, if Windows 10 is already installed, from either the Sign on screen or the Start menu, select Power (Power button icon) > hold Shift while selecting Restart. Select Troubleshoot > Advanced options > UEFI Firmware settings._
"

To elaborate on those instructions, it is hard to know what the magic key is for your computer to enter the BIOS menu, so you might as well try them all.  This might take a few tries.  A method that I have successfully used is the following: As soon as the computer restarts, press down the F1 key and then drag your your hand accross the F keys F2, F3, etc up to F11, F12, then turn around and go back and forth until you find yourself in the BIOS menu.  This might not work on your first attempt because the short window of time that the computer is checking to see if you are pressing the magical key is very short and you might just by bad luck, be at the other end of the keyboard during that fraction of a second.  So again, this might take a few attempts and there is also an outside chance that on your particular computer, the magic key you need to hit is Esc or Del.  
    
The other method (for Windows 10), where you hold the Shift key down while you reset the computer, you have to continue holding the reset key down before clicking on reset, and keep holding down the reset button until you get to the new menu. This new menu is not the BIOS menu but it may lead you there if you can select "Troubleshoot", then "Advanced Options", then "UEFI Firmware Settings".  

Regarless of which way you chose, if you get to the Windows sign-in screen, that means that the method you tried didn't work, and you will need to reboot and try again.

### At the BIOS Menu

**Your mission now is to make your computer boot from a USB.  So if you see a place that lets you change the boot order, You might try to move "USB" to the top of that list, or as a fall back plan, move anything called "Windows Boot Manager" to the bottom of the list.  That way the computer will check every other available boot option before booting into Windows as usual.**

![image](https://user-images.githubusercontent.com/12129459/127760658-6768e28c-f78e-44d5-9626-14356f09e2d6.png)

Changing the boot order may have options that look like this...

<hr>

![image](https://user-images.githubusercontent.com/12129459/127760779-916ca1f0-a021-4bf3-9079-c5ed7b5cb6ee.png)

or in rare cases you might see something that looks more like this...

<hr>

![image](https://user-images.githubusercontent.com/12129459/127760842-e3e4956b-b46d-42ba-871a-1c07336ccc34.png)

Here is an example after I moved Windows Boot Manager to the bottom of the list. 

<hr>

Save changes and exit.  

Try that out.  Plug in your new Bootable USB and restart your computer. 

If that doesn't work, you might have to go back into your BIOS/Startup menu again and locate another option where you can select between _Legacy_ or _UEFI_.  I have had much more luck using _"Legacy"_. 

![image](https://user-images.githubusercontent.com/12129459/127760935-30fe2b81-5ebe-48b1-9ddd-816cea0deec5.png)

Here is what this looks like on my computer, but I will show a few other examples to illustrate how this question looks different on different computers. 

<hr>

![image](https://user-images.githubusercontent.com/12129459/127749798-c18f3332-92d1-411d-84b9-7be4d7ed127e.png)

To illustrate that this will look different on every computer. Above is a screenshot where in this case there is an option called _Legacy USB Support_ which has to be enabled. 

<hr>

![image](https://user-images.githubusercontent.com/12129459/127749772-a6191b07-6812-463b-ba94-bc6ef49f9b17.png)

And in this other case there is an option called UEFI/BIOS Boot Mode, and you have options to select either UEFI or Legacy.  

As I've mentioned, you will have to look through the options for your particular computer.  

### For MacOS 
For Mac, I found that 50% of the time all you had to do was hold down the 'option' key when you heard the startup chime noise.  

![image](https://user-images.githubusercontent.com/12129459/127761118-d275fd02-01a5-4a19-a3f6-bc9ae5536a2a.png)

This would bring you to a 'Startup Menu' where you could select either your harddrive, or your USB-UEFI Boot.  If you see two, try the second one first.  Just because. 

<hr>

This method worked on exactly half of the test macs that I had access to.  The other 50% of the time you had to do an extra step of rebooting this time holding Command-R to enter a seperate Utilities menu.  

![image](https://user-images.githubusercontent.com/12129459/127761047-7170dcbf-3bf7-4765-8268-066acba639d0.png)

From here, all of the options are Red-Herrings, none of them are helpful. 

<hr>

![image](https://user-images.githubusercontent.com/12129459/127761052-ffe190a7-955d-45af-b44a-1c5a4257cfb4.png)

From here, you would have to use the menu at the top of the screen to select Utilities > Startup Security Utility.  

<hr>

Then you would have to change the two radio buttons to say "No security" - so it wasn't limited to ONLY booting into Official Mac Operating systems, and the button below for "Allow" booting from USB devices. 

![image](https://user-images.githubusercontent.com/12129459/127761099-3bc2af40-b154-4442-a909-6687ec43c931.png)

With those checkboxes in place, the previous instructions of reboot (with the boot USB already plugged in) then holding down the Option key when you hear the chime worked just fine.  

 


