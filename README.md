Cheat Sheet

# kpartx - Mount whole disk image as loopback per partition
kpartx -l disk.img

kpartx -a disk.img

kpartx -d disk.img

-l, --list

           List the partitions. Note that all numbers are in 512-byte sectors. This output format
           is DEPRECATED in favour of --show. Do not use it in newly written scripts.
           
-a, --add

           Add the specified partitions, or read the disk and add all partitions.
           
-d, --delete

           Delete the specified partitions or all partitions. It is not error to remove
           non-existing partitions, so this option is possible to use together with large --nr
           ranges without care about the current partitions set on the device.


