
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
- `df` 