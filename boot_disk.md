# Bootable USB Setup

The following instruction are provided in order to prepare Ubuntu boot disks. This is used when wishing to duel boot Ubuntu/Windows.

Instructions assume a Mac based laptop is being used to setup the Bootable USB

## Identifying the USB Disk 

Firstly identify the correct label for the USB drive.

```
diskutil list
```

This will respond with something similar to the following:

```
/dev/disk0 (internal, physical):
   #:                       TYPE NAME                    SIZE       IDENTIFIER
   0:      GUID_partition_scheme                        *121.3 GB   disk0
   1:                        EFI EFI                     209.7 MB   disk0s1
   2:                 Apple_APFS Container disk1         121.1 GB   disk0s2

/dev/disk1 (synthesized):
   #:                       TYPE NAME                    SIZE       IDENTIFIER
   0:      APFS Container Scheme -                      +121.1 GB   disk1
                                 Physical Store disk0s2
   1:                APFS Volume Macintosh HD            111.4 GB   disk1s1
   2:                APFS Volume Preboot                 44.5 MB    disk1s2
   3:                APFS Volume Recovery                517.0 MB   disk1s3
   4:                APFS Volume VM                      1.1 GB     disk1s4

/dev/disk2 (external, physical):
   #:                       TYPE NAME                    SIZE       IDENTIFIER
   0:      GUID_partition_scheme                        *30.8 GB    disk2
   1:                        EFI EFI                     209.7 MB   disk2s1
   2:                  Apple_HFS USBDISK                 30.4 GB    disk2s2
```


In the above we can see that the `/dev/disk2` label is 30GB in size and that is our USB stick.

## Erasing the USB Drive

Using the correct label, in order to fully erase the USB drive, use the following command:

```
diskutil eraseDisk JHFS+ USBDISK /dev/disk2
```

This gives the Drive a new name of **USBDISK** and puts the Mac OS Extended Journaled (JHFS+) filesystem on the drive.

## Download USB ISO

Head to the Ubuntu website and download the latest LTS version ISO.

https://www.ubuntu.com/download/desktop

## Download Etcher

Etcher is a tool for creating bootable disk.

https://www.balena.io/etcher/

## Create USB Disk

Once you have downloaded and installed Etcher, you can open it to create a bootable USB.

Choose the (downloaded) Ubuntu ISO, your USB drive as the target and click **Flash**
