# Syncloud.OS-HDD
Install in a "new" old computer HDD or SSD

Download the OS image x64 Syncloud OS;
Write the image like described here https://github.com/syncloud/platform/wiki ;
Start the computer with the USB (select the appropriate start mode from your BIOS);
Login with default credentials for non-activated device. Login: root, password: syncloud ;

Assuming you have only one SSD/HDD in your computer, use this command:

sudo dd if=/dev/sdb of=/dev/sda bs=4096 conv=noerror,sync

This will take a while. After doing it restart your computer with:

sudo shutdown -r now

Before any app install, expand the file system to take real disk size in Settings - Storage - Expand.

And it´s done.
