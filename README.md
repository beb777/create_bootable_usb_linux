# create_bootable_usb_linux
* identify the disk name 
  - `sudo fdisk -l`
 * make bootable depend up on thedistribution 
  - `sudo dd bs=4M if=Downloads/distubutionfilename.iso of=/dev/sdx status=progress && sync` # where x is disk name 
      * for example  for fedora 33 
        - `sudo dd bs=4M if=Downloads/Fedora-Workstation-Live-x86_64-33-1.2.iso of=/dev/sdb status=progress && sync` # where Fedora-Workstation-Live-x86_64-33-1.2.iso a distrubtion 
that i  download  with disk name is b in my case 
