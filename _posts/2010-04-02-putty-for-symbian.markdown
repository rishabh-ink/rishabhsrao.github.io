---
comments: true
date: 2010-04-02 20:11:00
layout: post
slug: putty-for-symbian
title: PuTTY for Symbian
wordpress_id: 35
categories:
- Tutorial
---

My experiences with PuTTY on my Nokia E63 and my openSUSE 11.2  desktop computer! 

Today I discovered a new amazing thing! I was able to connect to my desktop computer, over WiFi, from my mobile!

Here's how I did it! This also acts like a tutorial to anyone, who is new to the world of SSH!
[
](http://rishabhsrao.files.wordpress.com/2010/04/startyast.jpeg)Things you'll need



	
  1. A desktop computer (if you're running a Linux distro, then better!) (and if you're running [openSUSE 11.2](http://www.opensuse.org/):KDE even better!) (that's what I have!)

	
  2. A Nokia (Symbian series 60) mobile phone ([a list of compatible phones is here](http://en.wikipedia.org/wiki/S60_%28software_platform%29))

	
  3. A wireless modem


	
  4. Some basic knowledge on how to use Linux's KDE environment, nothing much!



Okay, so let's get started


You'll need to first install openSUSE 11.2 on your computer! There's an amazing newbie guide to openSUSE 11.2 at [http://opensuse-guide.org/](http://opensuse-guide.org/). Go and read it; you'll learn everything about openSUSE (including how to install and stuff!) 

Be sure you keep your wireless modem turned on and connected to your computer. So that openSUSE can automatically configure everything for you!

So, now that you've successfully installed openSUSE, sit back, relax and enjoy the beautiful KDE 4.3 desktop! Here's my desktop:

[![](http://rishabhsrao.files.wordpress.com/2010/04/startyast.jpeg?w=300)](http://2.bp.blogspot.com/_XVBkdaMWiEc/S7YCKr5jhUI/AAAAAAAAACY/-7Y4upcc424/s1600/desktop.jpeg)
I know, I know, you just can't get your eyes off your breathtaking KDE 4.3 desktop, but you'll have to now look at your mobile phone, because we're now gonna install PuTTY on your Symbian phone!

Simply visit [http://s2putty.sourceforge.net/](http://s2putty.sourceforge.net/) and go to the [Download section](http://s2putty.sourceforge.net/download.html). Here, download the appropriate installation file for your phone. You now need to transfer the .SIS installation file to your phone:



	
  1. Connect your phone in Mass Storage mode[![](http://rishabhsrao.files.wordpress.com/2010/04/screenshot00413.jpg?w=300)](http://rishabhsrao.files.wordpress.com/2010/04/screenshot00413.jpg)

	
  2. Hey, wait a minute, do you seriously need step-by-step instructions for transferring files?? I mean, come on, you can do this bit on your own!



After installing PuTTY, you should see the PuTTY icon in your Installations folder. 

Now, come back to your computer. We now need to verify whether the SSH daemon is up and running.




	
  1. Click the green SUSE lizard logo on your Plasma  panel.

	
  2. Roll your mouse over Computer.

	
  3. Click on YaST (Administrator Settings.)[![](http://1.bp.blogspot.com/_XVBkdaMWiEc/S7YJzX8DmmI/AAAAAAAAACg/ZLGSKdqpLDE/s400/start+yast.jpeg)](http://rishabhsrao.files.wordpress.com/2010/04/startyast.jpeg)

	
  4. If prompted for the root password, enter it and say OK.

	
  5. The YaST control panel shows up.

	
  6. Now, click on System in the left-side panel, and then click on System Services (Runlevel) under System on the right-side.[![](http://rishabhsrao.files.wordpress.com/2010/04/ssh.jpeg?w=300)](http://rishabhsrao.files.wordpress.com/2010/04/ssh.jpeg)

	
  7. In the System Services window, scroll down until you see sshd. That's the SSH daemon. Select it and click on the Enable button below and you should get a pop-up window saying the the return value was 0 (success.) That's all. Now dismiss that pop-up window and say OK to the System Services window.


Come back to the YaST control panel window.We need to add an exception to your computer's firewall so that it allows SSH connections. Here's how you do it: 

WARNING: What you are about to do is open the SSH port  (22) on your computer. Anybody can connect to your computer using  SSH, if this port is not protected by your firewall. 

I highly recommend that you remove your telephone line from  your modem now, so that you are safely disconnected from the Internet.

If you do this, you should be safe (except for local hackers who are within your modem's WiFi range!)
[
](http://rishabhsrao.files.wordpress.com/2010/04/startyast.jpeg)



	
  1. On the left-side panel, click on Security and Users, and then on the right-side, click on Firewall, under the Security and Users section.[![](http://rishabhsrao.files.wordpress.com/2010/04/firewallatyast3.jpeg?w=300)](http://rishabhsrao.files.wordpress.com/2010/04/firewallatyast3.jpeg)

	
  2. Under the Firewall Configuration window, in the left-side panel, click on Allowed Services.

	
  3. Under the Service to Allow drop-down combo box, select Secure Shell Server.[![](http://rishabhsrao.files.wordpress.com/2010/04/sshdropdowncombobox.jpeg?w=300)](http://rishabhsrao.files.wordpress.com/2010/04/sshdropdowncombobox.jpeg)

	
  4. Now click on the Add button at the right-side. Notice that Secure Shell Server gets added to the list below.


	
  5. Click on Next button at the bottom-right-side of the window.

	
  6. You will now see a summary of the settings that are going to change. Click Finish and your openSUSE will perform the firewall setting changes.


Congratulations, you can now connect to your computer via SSH.

Just one last thing, you'll need to know your desktop computer's IP address. So open Terminal, it should be under green lizard icon >> Favorites section.

In here, type the following command:

/sbin/ifconfig 

Here's what I see...

[![](http://rishabhsrao.files.wordpress.com/2010/04/ifconfig.jpeg?w=300)](http://rishabhsrao.files.wordpress.com/2010/04/ifconfig.jpeg)
Under eth0, on the second line,  there's this inet addr:, isn't it? Note the IP address written next to it. That's your computer's IP address. You'll need to enter this address in PuTTY.


Let's get back to PuTTY on your Symbian mobile phone

Here are the step-by-step instructions to connect to your openSUSE computer from your mobile phone: 




	
  1. Start PuTTY from the Installations folder.[![](http://rishabhsrao.files.wordpress.com/2010/04/screenshot0009.jpg?w=300)](http://rishabhsrao.files.wordpress.com/2010/04/screenshot0009.jpg)

	
  2. Select Default.

	
  3. PuTTY will now ask you to enter the hostname of the computer you wanna connect to.[![](http://rishabhsrao.files.wordpress.com/2010/04/screenshot0023.jpg?w=300)](http://rishabhsrao.files.wordpress.com/2010/04/screenshot0023.jpg)

	
  4. Remember the IP address that you had noted down earlier? Type in the same here.

	
  5. Now, it's gonna ask you about which Access Point to use. Be sure your modem access point is defined in your phone. If not, the select Search for WLAN, select your modem's wireless network name (SSN) and optionally, enter the WEP/WPA2 key. By doing this, you'll be defining a new Access Point.[![](http://rishabhsrao.files.wordpress.com/2010/04/screenshot0024.jpg?w=300)](http://rishabhsrao.files.wordpress.com/2010/04/screenshot0024.jpg)

	
  6. Now PuTTY will attempt to connect to your computer.[![](http://rishabhsrao.files.wordpress.com/2010/04/screenshot0025.jpg?w=300)](http://rishabhsrao.files.wordpress.com/2010/04/screenshot0025.jpg)

	
  7. Once it's connected, it'll prompt you the enter the Login Name. Enter your openSUSE login name (user name) here.[![](http://rishabhsrao.files.wordpress.com/2010/04/screenshot0026.jpg?w=300)](http://rishabhsrao.files.wordpress.com/2010/04/screenshot0026.jpg)

	
  8. I use root so that I get full access rights. This is not a recommended approach.

	
  9. It'll now prompt you to enter the password. So, enter the password for that user.[![](http://rishabhsrao.files.wordpress.com/2010/04/screenshot0027.jpg?w=300)](http://rishabhsrao.files.wordpress.com/2010/04/screenshot0027.jpg)

	
  10. Congratulations, you've successfully connected to your openSUSE computer via SSH![![](http://rishabhsrao.files.wordpress.com/2010/04/screenshot0028.jpg?w=300)](http://rishabhsrao.files.wordpress.com/2010/04/screenshot0028.jpg)


You can now use all the regular shell commands! Your mobile phone acts like a dumb terminal. If you wanna send special keystrokes, like ESC etc., that click Send and a list of keystrokes will appear.

I haven't figured out a way to transfer files between my computer and my mobile phone yet. There's a Java application called MobyExplorer and it has FTP support. Once I find out more about it, I'll blog it here!

Thank you for reading my blog and happy SSH-ing!

Post a comment if you have any doubts. I'll be happy to help you out! 

Here are some more screen-shots of me using PuTTY!

Here's a the popular ls command in action!

[![](http://rishabhsrao.files.wordpress.com/2010/04/screenshot0029.jpg?w=300)](http://rishabhsrao.files.wordpress.com/2010/04/screenshot0029.jpg)

Here's where I create a file called hello.txt using the cat command and the shell's here document, <, operator. I later display the contents of hello.txt using cat.

[![](http://rishabhsrao.files.wordpress.com/2010/04/screenshot0030.jpg?w=300)](http://rishabhsrao.files.wordpress.com/2010/04/screenshot0030.jpg)

And this is the best part! You can actually use the vi editor and do programming!

[![](http://rishabhsrao.files.wordpress.com/2010/04/screenshot0031.jpg?w=300)](http://rishabhsrao.files.wordpress.com/2010/04/screenshot0031.jpg)

I'm typing the program using my QWERTY keypad! Notice that I use the Send option to send special characters, in this case, the Tab character.

[![](http://rishabhsrao.files.wordpress.com/2010/04/screenshot0032.jpg?w=300)](http://rishabhsrao.files.wordpress.com/2010/04/screenshot0032.jpg)
I'm done typing my hello-world C program!

[![](http://rishabhsrao.files.wordpress.com/2010/04/screenshot0033.jpg?w=300)](http://rishabhsrao.files.wordpress.com/2010/04/screenshot0033.jpg)

Time to save and quit!

[![](http://rishabhsrao.files.wordpress.com/2010/04/screenshot00341.jpg?w=300)](http://rishabhsrao.files.wordpress.com/2010/04/screenshot00341.jpg)

As you can see, my C program, hello.c has been created!

[![](http://rishabhsrao.files.wordpress.com/2010/04/screenshot00351.jpg?w=300)](http://rishabhsrao.files.wordpress.com/2010/04/screenshot00351.jpg)

Let me just compile that program using g++.

[![](http://rishabhsrao.files.wordpress.com/2010/04/screenshot00361.jpg?w=300)](http://rishabhsrao.files.wordpress.com/2010/04/screenshot00361.jpg)

There you have it, g++ has conveniently create the executable file, a.out for me!

[![](http://rishabhsrao.files.wordpress.com/2010/04/screenshot00371.jpg?w=300)](http://rishabhsrao.files.wordpress.com/2010/04/screenshot00371.jpg)

Let's execute it, shall we?

[![](http://rishabhsrao.files.wordpress.com/2010/04/screenshot00381.jpg?w=300)](http://rishabhsrao.files.wordpress.com/2010/04/screenshot00381.jpg)

And here's the output of our program!

[![](http://rishabhsrao.files.wordpress.com/2010/04/screenshot00391.jpg?w=300)](http://rishabhsrao.files.wordpress.com/2010/04/screenshot00391.jpg)
That's the combined power of Linux, SSH and Symbian, baby! Symbian rocks!

That's all from me this time! Stay tuned for more!
