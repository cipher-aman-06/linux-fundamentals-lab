
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
- `fsck` → checks and reapirs