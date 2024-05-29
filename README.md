The following is the different customization that i do for my arch install:
1. Disabling the beep noise :
	
	Simply do 
	```
	sudo rmmod pcspkr
	sudo rmmod snd_pcsp
	```
	Don't worry if it gives the error snd_pcsp is not currently loaded.

	Then to prevent the modules from loading the next boot cycle create ```
	/etc/modprobe.d/nobeep.conf``` and add
	```
	blacklist pcspkr
	blacklist snd_pcsp
	```
 	to disable loading of the moudules on further boot-ups.




2. To make sure that files of a torrent are visible in KTorrent:
	
	Install the geoip program using ```sudo pacman -S geoip```
