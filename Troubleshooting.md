# Troubleshooting and FAQs

[Fatal: No bootable medium found! System halted](#fatal-boot-error)
<br>

[Forgot Password Easy Mode ](#forgot-password-easy-solution )

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


### Forgot Password - Easy solution 
Note: This method may not be available for your particular installation of Ubuntu.  


![image](https://user-images.githubusercontent.com/12129459/126672924-1d212347-a57d-4cd0-8769-3d1a07f6a857.png)


### Fatal Boot Error 

Harder way 



