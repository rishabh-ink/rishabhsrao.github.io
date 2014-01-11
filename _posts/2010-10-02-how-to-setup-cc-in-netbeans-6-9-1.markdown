---
comments: true
date: 2010-10-02 12:08:27
layout: post
slug: how-to-setup-cc-in-netbeans-6-9-1
title: How to setup C/C++ in NetBeans 6.9.1
wordpress_id: 136
---

This article is a step-by-step tutorial to help you set up C/C++ in your NetBeans 6.9.1 IDE on your openSUSE 11.2 OS. These instructions should be easy to modify for any GNU/Linux-based OS too!


## Things You'll Need





	
  * NetBeans 6.9.1 - The Smart Way to Code

	
  * openSUSE 11.2 (But any GNU/Linux-based OS will do!)

	
  * A Terminal window




## First Steps...


Let's install the required tools from the GNU Compilers Collection. Here is a list of tools that you'll need:



	
  * C Compiler: **gcc**

	
  * C++ Compiler: **g++**

	
  * Assembler: **as**

	
  * Make Command:** gmake**

	
  * Debugger Command: **gdb**

	
  * CMake Command: **cmake** (I think this one is optional; but I'm not sure! So let's install it anyway!)


At your terminal window, enter the following command,

    
    sudo zypper install gcc gcc-c++ binutils gmake gdb cmake


**zypper** is the package manager used by openSUSE 11.2 at the terminal. For Ubuntu, you might have to enter something like,

    
    sudo apt-get install gcc gcc-c++ binutils gmake gdb cmake


I'm not sure, just check on the Internet.

Moving on, enter your **root** password and let **zypper** (or your package manager) install the necessary packages.


### Setting up NetBeans...


Once you're done, follow the steps below:



	
  1. Open your NetBeans IDE and goto **Tools** > **Options**.

	
  2. Click on the **C/C++** tab.

	
  3. You should see a window similar to the one below, but with empty fields.

	
  4. [![](http://rishabhsrao.files.wordpress.com/2010/10/netbeans_options_candc.png)](http://rishabhsrao.files.wordpress.com/2010/10/netbeans_options_candc.png)Click on the **Add...** button near the bottom-left corner.

	
  5. Enter the **Base Directory** as **/usr/bin** and press the **Tab** key.

	
  6. NetBeans will automatically select the **Tools Collection** name as **GNU** from the combo-box.

	
  7. Enter a nice name at the **Tools Collection Name** like **GNU Compiler Collection** or something.[![An image showing the NetBeans - Add New Tools Collection window.](http://rishabhsrao.files.wordpress.com/2010/10/gcctoolscollection.png)](http://rishabhsrao.files.wordpress.com/2010/10/gcctoolscollection.png)

	
  8. Click **OK**.

	
  9. Your **Options** window should now look similar to the **Options** window image shown above (after step 3.)

	
  10. Congratulations, your NetBeans IDE should now be ready to run C/C++.




### Further help...


Comment back here if you need any help regarding this. I'd be happy to help!


### Happy Programming!


If you have any suggestions for improvements, please comment!
