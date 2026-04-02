
---
## Question 1
Attach a USB drive to the system and then safely detach it using Linux commands.
### Approach
First identify the USB device path, mount it to a directory, then unmount it after use.
### Commands
- `lsblk` → shows connected storage devices
- `mount` → attach device to directory
- `unmount` → safely detach device
### Output
##### STEP 1 : identify usb device
![[Pasted image 20260401072343.png]]
##### STEP 2 : mount usb drive
![[Pasted image 20260401072720.png]]
##### STEP 3 : unmount usb drive
![[Pasted image 20260401072759.png]]
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
![[Pasted image 20260401072953.png]]
### Key Observations
Primary disk usually mounted on root(/).
-h flag shows size in GB/MB.
### What I learned
Disk usage monitoring helps prevent storage exhaustion.

---
## Question 3
Clone full data from one USB device to another including hidden or deleted content.
### Approach
Use low-level copy command to duplicate raw disk blocks.
### Commands
- `dd` → copies raw data bit-by-bit
- `lsblk` → identify device names
#### Output
##### STEP 1 : identify devices
![[Pasted image 20260401075308.png]]
##### STEP 2 : copy disk content
![[Pasted image 20260402222006.png]]
### Key Observations
dd copies raw blocks, not files.
Deleted data may still exist in disk sectors.
### What I learned
Bit-level cloning is useful in digital forensics.

---
## Question 4
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
2. Monitoring disk usage prevents denial-of-service via storage exhaustion.
3. Raw disk cloning allows forensic recovery of deleted evidence.
4. Block device enumeration reveals system storage attack surface.

---
