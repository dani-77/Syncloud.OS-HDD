# Syncloud.OS-HDD
Install in a "new" old computer HDD or SSD

Download the OS image x64 Syncloud OS from here https://github.com/syncloud/platform/wiki and and write it to a USB flash drive following the instructions in the same page;
Start the computer with the USB (select the appropriate boot device from your computer BIOS);
Login with default credentials for non-activated device. Login: root, password: syncloud ;

Assuming you have only one SSD/HDD in your computer, use this command:

sudo dd if=/dev/sdb of=/dev/sda bs=4096 conv=noerror,sync

This will take a while, but after running it, the system is on the HDD or SSD. Turn off your computer with:

sudo shutdown now
Power it up again, select the boot device again from your BIOS, but to start the HDD/SSD.

Before any app install, expand the file system to take real disk size in Settings - Storage - Expand.

And it´s done.
