---
comments: true
date: 2010-01-10 17:42:00
layout: post
slug: javafx-a-tutorial-for-newbies
title: 'JavaFX: A Tutorial for Newbies!'
wordpress_id: 30
categories:
- Tutorial
---

After learning JavaFX for a few days, I decided to create my first JavaFX application! It's called Open-Source Jumble and I'm happy to say that it's up to the coveted version 1.0.0 now! Here is a screen shot of my application:


[![](http://rishabhsrao.files.wordpress.com/2010/01/jumble_app_snapshot1.jpeg?w=175)](http://rishabhsrao.files.wordpress.com/2010/01/jumble_app_snapshot1.jpeg)
For all you curious readers out there, the font used for the title is [Letras Locas](http://www.kde-look.org/content/show.php/Letras+Locas?content=116231) available at [KDE-Look.org](http://www.kde-look.org/) and for all you curious folks reading this, I'm running [openSUSE](http://www.opensuse.org/) 11.2 ([KDE](http://www.kde.org/)) with the [Aurorae theme engine](http://www.kde-look.org/content/show.php/Aurorae+Theme+Engine?content=107158)! The window decoration theme is [Kant2](http://www.kde-look.org/content/show.php/Kant2+Aurorae?content=115339). 

Read more about this application in my other blog at [http://osum.sun.com/profiles/blogs/jumble-javafx-style](http://osum.sun.com/profiles/blogs/jumble-javafx-style)!

So, now in the spirit of open-source, I'm going to teach you the basics of JavaFX in a simple, easy to follow, step-by-step tutorial. We'll start with a simple "Hello World" application and then gradually move on to more advanced stuff.

So, here we go! I'll write this blog as a conversation between you and me!

You: Wow, your application looks good! Can I too develop such applications? But I don't know anything about JavaFX! :(
Me: Thank you! Yes, sure you can! Don't worry, you're in the right place! :)

You:  Okay, so what is JavaFX?
Me: JavaFX is a new Rich **I**nternet Application (RIA) development platform, created by Sun Microsystems, where you can create visually attractive applications easily.

You: Oh, I see. Where is the JavaFX website located?
Me: Please see [http://javafx.com/](http://javafx.com/) and  [http://javafx.com/docs/gettingstarted/javafx/](http://javafx.com/docs/gettingstarted/javafx/) will answer you previous question more precisely.

You: What all can I do with JavaFX?
Me: JavaFX is a very powerful platform. Check out [http://javafx.com/samples/](http://javafx.com/samples/) to see some amazing applications developed in JavaFX!

You: Cool! Those sample applications are awesome! I too wanna learn JavaFX!
Me: Yes, they're are indeed awesome! They were developed using JavaFX. So, shall we start then?

You: You bet! What do I do first?
Me: The easiest way to start off JavaFX is to use an IDE (Integrated Development Environment) like [NetBeans](http://netbeans.org/)! Get NetBeans version 6.8 or later: JavaFX at the [NetBeans IDE Download](http://netbeans.org/downloads/index.html) page. Click on the Download button under the JavaFX column. It's 78MB, so use a download manager. If you have a slow internet connection, consider requesting a CD/DVD from your institution's [Sun OSUM](http://osum.sun.com/) club. Or ask one of your friends, who has broadband internet, to download it for you.

After downloading, read [NetB](http://netbeans.org/community/releases/68/install.html)[eans 6.8 IDE Installation Instructions](http://netbeans.org/community/releases/68/install.html) and install it on your computer. Before you install, please note that you need to have the latest Java SE Development Kit (JDK) installed on your system. Visit [http://java.sun.com/javase/downloads](http://java.sun.com/javase/downloads) for more information. Also, be sure to enable the Features On Demand feature while installing. It'll make the IDE start up faster.

You: Hey I installed NetBeans! How do I start creating applications?
Me: Start the NetBeans IDE. After it finishes loading the required modules, you'll see the NetBeans Start Page. Explore the Start Page, if you like to learn more about NetBeans.

Follow the steps below:
1. Click File >> New Project...
2. Under the Choose Project >> Categories
3. Now, under the Projects pane, click on JavaFX Script Application and click Next >
You'll see a window like this:

[![](http://rishabhsrao.files.wordpress.com/2010/01/newproject2.jpeg?w=300)](http://rishabhsrao.files.wordpress.com/2010/01/newproject2.jpeg)
4. Give the Project Name as "HelloJavaFX" (or any other name you like!)
5. Be sure the Set as Main Project and Create Main File: [hellojavafx.Main] check-boxes are checked
6. Click Finish

and you're done!

You: Alright! I did that!
Me: Good! As you can see, NetBeans has set up everything for you. It has even created a small JavaFX application template. You have a minimal, but complete JavaFX application in front of you. If you'd like to run it and see now, simply click the Run button (it looks like a green play button found on media players!) above.

NetBeans will build the application and you'll see a new window titled Application title on your screen. There's also Application content written inside!

All JavaFX files end with a .fx extension, like your Main.fx file.

You can change the window title by changing the title of your Stage object literal. You can also modify the text inside the window by modifying the content of the Scene object literal.

There you have it, your first, simple "Hello World" JavaFX application!

I'll write more tutorials about JavaFX in the coming future! So, Follow me for more!


