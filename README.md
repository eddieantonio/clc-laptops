Things to do to setup loaner laptops
====================================

Here are instructions on how I set up our loaner laptops.


Quick facts: What is the default user account?
----------------------------------------------

Username: `Learner`
Password: `canadalearningcode`


Why set up the laptops with Lubuntu?
------------------------------------

Running Windows 10 on the 32GB HP Stream was painful; they hardly had
enough storage to download Windows 10 updates. We got "disk out of
space" error messages when saving text files.

[Lubuntu][] is a small, lightweight distribution of Linux, based on
Ubuntu, with a bare bones desktop environment. The installation of
Lubuntu with all required software used under 6 GiB of storage.



Packages required for workshops

 - Chromium
 - Atom
 - Python 3
 - Ruby (as offline contingency during for the Repl.it Ruby workshop)
 - Scratch 2 (as offline contingency during for the Scratch workshops)
 - ~~Processing~~ (Not installed because set up on Linux is tricky!)


Installing (most) of the required software
------------------------------------------

Run `./install-all`

Instructions
------------

To install [Lubuntu][] on HP Stream 14:

[Lubuntu]: https://lubuntu.me/

 - Download a 64-bit version of Lubuntu. 32-bit will not work! (due to
   BIOS/UEFI incompatibility... or something).
 - Using a tool like [Unetbootin](https://unetbootin.github.io/),
   write the ISO to a USB drive.
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
 - Turn off Bluetooth.
 - Add icons to Desktop.
 - Background: Canada Learning Code logo
 - Desktop: icons for Chromium, Atom, Scratch
