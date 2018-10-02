# Basic guidelines on how to run ifd68 programming app on a Mac

## Background

All the emulation frameworks I tried; Crossover, Wine, etc. were able to run
the program, but failed to get direct access to the keyboard when plugged into
USB. Success was found with a combination of VirtualBox, IE8 VM images, and the
software on this page.

## What you need:

  - ifd tools courtesy of GonzaloAlvarez: https://github.com/GonzaloAlvarez/ifd68
  - Some handy instructions, most of which apply for the Mac version of VirtualBox: https://sites.google.com/site/easylinuxtipsproject/oldgrub
  - Free and totally legal IE images (I used IE8) from Microsoft: https://developer.microsoft.com/en-us/microsoft-edge/tools/vms/
  - Some more good tips on installing the images: https://sites.google.com/site/easylinuxtipsproject/oldgrub

## Steps

Extremely abbreviated and probably incomplete instructions for legally reprogramming your Keywalker IFD68 on a Mac:

  - Clone https://github.com/GonzaloAlvarez/ifd68 to your Mac.
  - Download and install VirtualBox.
  - Download and install free IE8 VM image from Microsoft website into VirtualBox.
  - Install Virtual Box tools to VM via menu Devices - Insert Guest Additions CD .
  - Reboot as needed.
  - Share cloned ifd68 directory through VirtualBox (shared folders).
  - Plug in IFD68 keyboard to USB port.
  - Add IFD68 keyboard to VM via menu Devices - USB.
  - Navigate to shared ifd68 directory in the VM, it's on the network
  - Run fd68/software/original/programmer/IFD68.exe and Bob's your uncle!

Many thanks to GonzaloAlvarez, Oracle, and Microsoft for providing the tools needed for this.
