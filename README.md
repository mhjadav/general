# General

# Set RD/WR permission for external hard disk
	• Uninstall other 3rd-party NTFS software, like Paragon, Tuxera or NTFS-3G.
	
	• Edit /etc/fstab (you can do this with “ sudo vi /etc/fstab ”)
	
		○ Add the following line:
		
    			# LABEL=VolumeName none ntfs rw,auto,nobrowse
			
		○ Quit your editor
		
	• Now, just unmount and re-mount the disk
	
	• And we are done! You now have read-write support for this disk in OSX
	

# To open 

open /Volumes/VolumeName

# To Unmount
diskutil unmount /Volumes/VolumeName
