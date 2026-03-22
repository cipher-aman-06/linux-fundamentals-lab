
---
## Question 1
Explore the Linux directory structure starting from the root directory and verify navigation using commands.

### Approach
I started from the root directory '/' and used commands to list available directories. Then I navigated into each directory and verified my location using the 'pwd' command.

### Commands
- `cd /` moves to the root directory
- `ls`lists files and directories inside the current directory.
- `cd <directory>` is used to navigate into a specific directory
- `cd ..` is used to move one directory back (parent directory)
- `pwd` confirms the current working directory
### Output

##### STEP 1 : Move to the root directory
![[Pasted image 20260322090407.png]]
##### STEP 2 : List root directories
![[Pasted image 20260322093513.png]]
##### STEP 3 : Navigate to /bin and verify working directory
![[Pasted image 20260322094901.png]]
##### STEP 4 : Move one directory back (parent directory) and navigate to /etc and verify working directory
![[Pasted image 20260322095201.png]]
##### STEP 5 : Direct navigate to /etc to /home and verify working directory
![[Pasted image 20260322095246.png]]
### Key Directories Observed
- `/bin` → Essential user binaries  
- `/etc` → Configuration files  
- `/home` → User directories  
- `/var` → Logs and variable data
### What I Learned  
Linux uses a hierarchical filesystem starting from root (/).