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
-------------------------------

 - Chromium
 - Atom
 - Python 3
 - Ruby (as offline contingency during for the Repl.it Ruby workshop)
 - Scratch 2 (as offline contingency during for the Scratch workshops)
 - ~~Processing~~ (Not installed because set up on Linux is tricky!)


Instructions
------------

To install [Lubuntu][] on HP Stream 14:

[Lubuntu]: https://lubuntu.me/

### Creating the bootable USB drive

 - Download a 64-bit version of Lubuntu. 32-bit will not work! (due to
   BIOS/UEFI incompatibility... or something).
 - Using a tool like [Unetbootin](https://unetbootin.github.io/),
   write the ISO to a USB drive.

### Initiating the Lubuntu install

 - Mash the <kbd>ESC</kbd> when booting up the machine. The BIOS's
   default settings leave very little time to do this properly.
 - At the options screen, press <kbd>F9</kbd> to select the boot device.
 - Select the USB drive as the bootable device; do not choose the hard
   drive!

### Installing Lubuntu

During the installer, take the following options:

 - Keyboard: English (US) layout
 - Choose: Minimal installation
 - Install third-party software for graphics and Wi-Fi hardware and additional media formats
 - Setup Secure Boot with an easy-to-remember one-time password;
   you'll need to enter it when rebooting after the installation.
 - Use LVM with the new Lubuntu installation
 - Username: `Learner`
 - Password: `canadalearningcode`
 - Computer name: "clc" + what it says on the sticker on the back of the lid.
 - Log in automatically

It should now install Lubuntu. Wait to reboot, and register the key
(password you entered for Secure Boot). Lubuntu should start up after the
reboot. Note: boot time is a bit slow.

### Configuring Lubuntu

After installing Lubuntu, install all of the required software, and
configure it for a better user experience.

#### Installing all of the software

In a terminal (System Tools » LXTerminal), do the following:

```sh
sudo apt install -y git  # Install git (pre-requisite).
git clone https://github.com/eddieantonio/clc-laptops.git
cd clc-laptops
./install-all  # Install all of the software!
```

#### Better user experience

 - Disable multiple desktops (confusing when you accidentally scroll on the desktop)
     - "Start" » Preferences » Openbox Configuration Manager » Desktop
 - Remove "Iconify all windows" panel button.
    - Right-click » Remove "..." from Panel
 - Turn off screen lock
     - "Start" » Preferences » Power Manager
         - General: On battery/Plugged in: suspend
         - Security: Automatically lock the session: never
 - Do not ask for password on login
     - "Start" » System Tools » Users and Groups
        - Learner/Password: Change... » ✔ Don't ask for password on login
 - Turn off Bluetooth. In the taskbar, click on Bluetooth and turn it off.
 - Add the following desktop icons: Chromium, Atom, Scratch
 - Set the background to the Canada Learning Code logo
