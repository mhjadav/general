# general

Set RD/WR permission for external hard disk
	• Uninstall other 3rd-party NTFS software, like Paragon, Tuxera or NTFS-3G.
	
	• Edit /etc/fstab (you can do this with “sudo vi /etc/fstab”)
	
		○ Add the following line:
		
    			# LABEL=”VOLUME_NAME_WITHOUT_QUOTES” none ntfs rw,auto,nobrowse
			
		○ Quit your editor
		
	• Now, just unmount and re-mount the disk
	
	• And we are done! You now have read-write support for this disk in OSX
	

#To open 

open /Volumes/VolumeName


Or you can use batch file in this directory to mount and unmount

Set path to your volume before you run file.
