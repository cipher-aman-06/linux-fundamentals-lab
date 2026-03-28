
---
## Question 1
Display detailed file permissions of a selected directory
### Approach
I selected a directory and used the long listing option to view detailed file information, including read, write, and execute permissions.
### Commands
- `ls` → lists directory contents
- `ls -l` → shows detailed file permissions
- `ls -la` → includes hidden files
### Output
##### STEP 1 : Navigate to directory
![[Pasted image 20260328222750.png]]
##### STEP 2 : Display long listing
![[Pasted image 20260329013518.png]]
##### STEP 3 : Display hidden files
![[Pasted image 20260329013558.png]]
### Key Observations
Each file shows permissions in this format : `-rwxr-xr-x`
### What I learned
Linux controls access using file permissions which define who can read. modify, or execute files.

---
## Question 