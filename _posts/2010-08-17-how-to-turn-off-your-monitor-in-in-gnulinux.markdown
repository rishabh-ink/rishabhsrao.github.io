---
comments: true
date: 2010-08-17 21:27:56
layout: post
slug: how-to-turn-off-your-monitor-in-in-gnulinux
title: How to turn off your monitor in in GNU/Linux
wordpress_id: 19
categories:
- Tutorial
---

Here's a handy tip to turn off your monitor and to save electricity & save the environment:

Just type

    
    xset dpms force off
    


in your shell!

This works with most operating systems, such as openSUSE, Ubuntu, Fedora etc. In other words, systems running the [X Window System](http://en.wikipedia.org/wiki/X_Window_System).

If you're running KDE + openSUSE 11.2 (like me!) then you can also create a button in your taskbar to do the above!

Here's how:



	
  1. Right-click on your **KDE Kickoff Application Launcher**.

	
  2. Select **Menu Editor**.

	
  3. In the categories displayed on your left, right-click **System** and select **New Item...**.

	
  4. When asked for a name, enter **Turn Off Monitor**.

	
  5. To your right, in the **General** tab, in the **Description** textbox, enter **Puts your monitor in standby mode**.

	
  6. Add a **Comment** if you fancy.

	
  7. Select an icon for your button by clicking the big button with the question mark.

	
  8. My personal favorite is the [![preferences-web-browser-shortcuts](http://rishabhsrao.files.wordpress.com/2010/08/turn-off-monitor.png)](http://rishabhsrao.files.wordpress.com/2010/08/turn-off-monitor.png) icon; but you can select any icon you fancy.

	
  9. To select my favorite icon, under the **Icon Source** select the **System icons **radio button, select **Applications** in the combo-box and search for **preferences-web-browser-shortcuts **and click **OK** (if necessary.)

	
  10. In the **Command** text-box, type **xset dpms force off**.

	
  11. Click on the **Advanced** tab and notice that the **Current Shortcut Key** has a **None** button.

	
  12. Click on that **None** button and press & hold the **Meta** (i.e. Windows) key and (while still holding it) press the **` **(back-quotes or the tilde) key. After you release both the keys, the key shortcut **Meta + `** should be visible instead of **None**.

	
  13. You're done! Just click **Save** on the **KDE Menu Editor**'s toolbar and close the window.

	
  14. The **Turn Off Monitor** menu command will now feature in the **Kickoff **> **Applications** > **System **menu.

	
  15. You can now:

	
    * Right-click on it and select **Add to Favorites**.

	
    * Drag and drop it onto your taskbar. (Be sure your KDE Plasma widgets are unlocked.)





That's all folks! Help protect our planet Earth in all the ways you can, however little your contribution may be.
