`RAID` - `Redundant Array of Independant Disks`

Seperate disks work together and acting like a one disk.

* __RAID 0__ - Striped, No redundancy, good performance.
* __RAID 1__ - Mirrored, Redundancy
* __RAID 5__ - Good for reads, bad for writes. __AWS does not recommend ever putting RAID 5's on EBS__
* __RAID 10__ - Combination of RAID 0 and 1, Striped & Mirrored, Good redundancy, good performance

When to use RAID volumes?
    * When you want to increase disk I/O.

How?
    * Create Windows instance with e.g. 3 EBS volumes (SSD)
    * Run the instance and go to `Disk Management`
    * Delete all except the root one
    * Create `Striped` (`Raid 0`) volume.

Taking a snapshat of a RAID array?

* __Problem__: Caches can be a problem due to the interdependencies of the array.

* __Solution__: Take an application consistent snapshot:
    * Stop the application from writing to disk
    * Flush all caches to the disk.
        * Freeze the file system.
        * Unmount the RAID array.
        * Shut down the associated EC2 instance.