Things to do to setup loaner laptops
====================================

Download copies of all current workshops: **TODO**

Default user account
--------------------

Username: `Learner`
Password: `canadalearningcode`

 - Background: Canada Learning Code logo
 - Desktop: icons for Chromium, Atom, Repl.it, IDLE

Install
-------

Run `./install-all`

Package list
------------

 - Chromium
    - \*
 - Scratch 2
    - Gamemaking and Circuitry with Scratch & MaKey MaKey
 - Ruby
    - Ruby workshop
 - Python 3
 - Atom
    - HTML & CSS for Beginners: Learn to Build a Multi-Page Website from Scratch
    - Webmaking with HTML & CSS
 - Processing — Setup on Linux is tricky!


Considerations
--------------

Turn off Bluetooth.

Add icons to Desktop.

Updating all of the workshop repositories
-----------------------------------------

Run `./update-workshops`

Instructions
------------

To Install Lubuntu on HP Stream 14:

 - <kbd>ESC</kbd> when starting up. Default settings have no delay.
 - Install Lubuntu:
   - English (US) layout
   - Minimal installation
   - Install third-party software for graphics and Wi-Fi hardware and additional media formats
   - Use LVM with the new Lubuntu installation
   - Computer name: "clc" + what it says on the sticker
   - Log in automatically
 - Disable multiple desktops (confusing when you accidentally scroll on the desktop)
     - "Start" » Preferences » Openbox Configuration Manager » Desktop
 - change boot back to UEFI mode?
 - Remove "Iconify all windows" panel button.
    - Right-click » Remove "..." from Panel
 - Turn off screen lock
     - "Start" » Preferences » Power Manager
        - General: On battery/Plugged in: suspend
	- Security: Automatically lock the session: never
 - Do not ask for password on login
     - "Start" » System Tools » Users and Groups
        - Learner/Password: Change... » ✔ Don't ask for password on login
