
---
## Question 1
Attack a USB drive to the system and then safely detach it using Linux commands.
### Approach
First identify the USB device path, mount it to a directory, then unmount it after use.
### Commands
- `lsblk` → shows connected storage devices
- `mount` → attach device to directory
- `unmount` → safely detach device
### Output
##### STEP 1 : identify usb device
##### STEP 2 : mount usb drive
##### STEP 3 : unmount usb drive
### Key Observations
Linux treats USB drives as block devices like /dev/sbd.
Unmounting prevents data corruption.
### What I learned
Devices must be mounted before accessing their files.

---
## Question 2
Find how much storage space is available on the main disk.
### Approach
Use a command that displays disk usage and free space in readable format.
### Commands
- `df` → shows disk free space
- `df -h` → human readable format
### Output
##### STEP 1 : check disk free space
### Key Observations
Primary disk usually mounted on root(/).
-h flag shows size in GB/MB.
### What I learned
Disk usage monitoring helps prevent storage exhaustion.

---
## Question 3
Scan the USB drive for file system issues and repair them.
### Approach
Use filesystem check utility on the device after unmounting it.
### Commands
- `fsck` → checks and repairs filesystem errors
- `umount` → required before running fsck
### Output
##### STEP 1 : unmount device
##### STEP 2 : scan for errors
### Key Observations
fsck should not run on mounted partitions.
It can detect corrupted filesystem structures.
### What I learned
Filesystem errors can be fixed using built-in Linux tools.

---
## Question 4
Clone full data from one USB device to another including hidden or deleted content.
### Approach
Use low-level copy command to duplicate raw disk blocks.
### Commands
- `dd` → copies raw data bit-by-bit
- `lsblk` → identify device names
#### Output
##### STEP 1 : identify devices
##### STEP 2 : copy disk content
### Key Observations
dd copies raw blocks, not files.
Deleted data may still exist in disk sectors.
### What I learned
Bit-level cloning is useful in digital forensics.

---
## Question 5
Display structure and details of storage devices connected to the system.
### Approach
Use a command that lists block devices and partitions.
### Commands
- `lsblk` → lists block devices
- `lsblk -f` → shows filesystem type
### Output
##### STEP 1 : view block devices
##### STEP 2 : view filesystem details
### Key Observations
Block devices include disks, USB, partitions.
Shows mount point and filesystem type.
### What I learned
Understanding storage layout helps in system administration.

---
### Security Insights
1. Improper mounting/unmounting can expose data corruption risks.
2. Monitoring disk usage prevents denial-of-service via storage exha