
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
##### STEP 2 : 