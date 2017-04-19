## Install Live USB from Mac ##

 Launch the following command in order to identify the usb drive:
 	diskutil list
 
 Suppose it is /dev/disk2.
 
 Then proceed to copy the image on the USB device.
 	dd if=kali-linux-2016.2-amd64.iso of=/dev/disk2 bs=512k
 
 Once dd has finished imaging the drive, it will output something that looks like this:
 	5823+1 records in
	5823+1 records out
	3053371392 bytes (3.1 GB) copied, 746.211 s, 4.1 MB/s

## FIx EFI ##

Mount the USB device and replace the EFI/BOOT/ folder with the one in this repository.

 
