URL: <https://bugs.launchpad.net/ubuntu/+source/xserver-xorg-video-amdgpu/+bug/1577074>
Original report:

```
Title:  [HP Pavilion 15] Intermittent black screens
Body:

I'm having a hard time tracing this down. I updated to Kubuntu 16.04 (from Kubuntu 15.10 - that was using the Linux Crimson 15.12 driver) a couple days ago on my notebook (HP Pavilion, A10-8700P APU), and ever since I've been having random black screens.

I started debugging the driver, then thought it might be a DPMS issue (it's not - I have DPMS fully disabled currently), and now I'm back to debugging the driver.

I don't have any remnants of the former closed Crimson display driver and never had an xorg.conf file (I made a small one that I'm using at the moment consisting of only a server layout to ensure screen savers, DPMS, etc are all off).

The Black screen can happen any time from the login screen until hours later. I can ssh into the system to shut it down. And just discovered that if I unplug the system from it's power brick, I can close the lid - the system will goto sleep. When I flip the screen back up, the system wakes up and the screen works again for 1-2 minutes.

I don't see any errors in the log files (well, outside some nasty looking ACAPI errors in dmesg).

HOT TO REPRODUCE:
Boot system and use normally or simply leave system alone. Blank screen will happen any time after x comes up.

EXPECTED RESULT:
Screen doesn't blank unless a screen saver or power saver kicks in.

SYSTEM INFO:
Purchased Dec 2015 (build date from BIOS - Aug 2015), HP Pavilion 15" notebook, AMD A10-8700P "Carrizo", 16GB RAM, 960GB SSD
```
