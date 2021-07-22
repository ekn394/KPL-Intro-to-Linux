# Troubleshooting and FAQs

[Fatal: No bootable medium found! System halted](#fatal-boot-error)
<br>

[Forgot Login Password ](#password-reset-method-1)

<hr>
 
### Fatal Boot Error 
"FATAL: No bootable medium found! System halted." 

![image](https://user-images.githubusercontent.com/12129459/124355494-74e09f80-dbdf-11eb-9e30-1dc4152dd88b.png)

This means that an operating system image was not successfully loaded.

### Fatal Boot Error Solution

![image](https://user-images.githubusercontent.com/12129459/124356539-824c5880-dbe4-11eb-97f1-24827da9967f.png)

<br>With the problematic VM selected (step 1 - shown above). Click on the _Settings_ button (step 2 - shown above).

![image](https://user-images.githubusercontent.com/12129459/124356379-c2f7a200-dbe3-11eb-8f79-c555c668da60.png)

On the left hand side, select _Storage_ (step 1 - shown above) and you should see that something called the "Controller: IDE" is set to "Empty" meaning that it has no disk image selected.  Click on the word _Empty_ (step 2 - shown above).  

Next, click on the blue disk shape (step 3 - shown above) to open up a drop down menu of choices and select the option called _"Choose a disk file"_ (step 4 - shown above)

From there, navigate your files to fine find your image file (it should end in .iso).  For me this file is called ubuntu-20.04.2.0-desktop-amd64.iso.  When you find your equivalent file (check your downloads folder).  Double click on it to select it.  

With that done, you should now see the name of your image file instead of the word "Empty" 
![image](https://user-images.githubusercontent.com/12129459/124356727-a2c8e280-dbe5-11eb-892f-3a97cbf0b46a.png)

Click Ok, to close this settings window. 

![image](https://user-images.githubusercontent.com/12129459/124356793-08b56a00-dbe6-11eb-8d7a-2461889780e8.png)

Finally, turn your VM off and on again.  I think the easiest way to do this is to right click on your VM and select _Reset_.

<hr>


### Password Reset Method 1
Note: This method may not be available for your particular installation of Ubuntu.  

Let's say you forgot your password to login. For this example, the user account is named 'evan'. 

![image](https://user-images.githubusercontent.com/12129459/126675234-44068b90-4cb8-4dfd-9a0b-fbd08c1fe67e.png)

The first thing to do is reset your machine. Then, when the screen goes black, hit the escape key repeatedly until you see a GNU GRUB menu like this. 

![image](https://user-images.githubusercontent.com/12129459/126675425-482aa6a4-5e70-48dd-b881-19ca2e3dea52.png)

Use the arrow keys to select the option for "Advanced options for Ubuntu" and press Enter.
 
![image](https://user-images.githubusercontent.com/12129459/126675546-f5463e5d-ee3e-474a-a6da-8aa94cd6343d.png)

On the next screen, select an option that ends with the words "recovery mode".  You might see several options that look similar, that's fine, it doesn't matter which one you use for this purpose, so just go with the first one that says "recovery mode" and press enter. 

![image](https://user-images.githubusercontent.com/12129459/126672924-1d212347-a57d-4cd0-8769-3d1a07f6a857.png)

After a few seconds you should find yourself at a "Recovery Menu".  
Select the option for '**root - Drop to root shell prompt**'

![image](https://user-images.githubusercontent.com/12129459/126673773-38ae6143-86f6-4f45-b5bd-2a68e335c77d.png)

If at this point you see a prompt that says 'Press Enter for maintenance', then good news, you are in what I call 'easy-mode', and you can simply press Enter.

![image](https://user-images.githubusercontent.com/12129459/126673994-5e2485fe-6883-4c0c-ad68-85978acbf3da.png)

You will then see a command line prompt that looks like root@<theMachineName>:~# 
This means that for the moment you are signed in as the super-user, 'root'. Root has administrative control over all accounts (including the one that you are locked out of).  
 
![image](https://user-images.githubusercontent.com/12129459/126674331-ca666838-b75e-4f4f-a89c-70fd21a13ab9.png)

At this point you can type the command **passwd yourUserNameHere**
In my case the user I want to change the password for is the user named 'evan', so I will type **passwd evan**

![image](https://user-images.githubusercontent.com/12129459/126674464-6d29a64d-cadf-426b-8441-57833eead280.png)

It will ask you to supply a new password for that user.  
It will ask you to retype that same password to confirm.  

That's it.  You are done resetting the password for that user.  
You can reboot your virtual machine now and you should be able to log in to that user using the new password you just set up. 

### Forgot Password Method 2

Sometimes you will not see the "Press Enter for maintenance" but you will instead see a prompt asking you to supply the root password.
 
To be continued...


