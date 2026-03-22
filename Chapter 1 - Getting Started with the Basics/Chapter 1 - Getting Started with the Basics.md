
---
## Question 1
Explore the Linux directory structure starting from the root directory and verify navigation using commands.

### Approach
I started from the root directory '/' and used commands to list available directories. Then I navigated into each directory and verified my location using the 'pwd' command.

### Commands
- `cd /` moves to the root directory
- `ls`lists files and directories inside the current directory.
- `cd <directory>` navigates into the specified directory
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
##### STEP 5 : Navigate from /etc to /home and verify working directory
![[Pasted image 20260322095246.png]]
### Key Directories Observed
- `/bin` → Essential user binaries  
- `/etc` → Configuration files  
- `/home` → User directories  
- `/var` → Logs and variable data
### What I Learned  
Linux follows a hierarchical filesystem structure that starts from the root directory (/), allowing organized storage of system and user files.

---
## Question 2
Verify the currently logged-in user using a Linux command.
### Approach
I used a command that displays the username of the active session to confirm which account is currently logged in.
### Command
- `whoami`→ displays current logged-in username
### Output
##### STEP 1 : check current user
![[Pasted image 20260322114009.png]]
### Key Observations
The command directly prints the username associated with the active session
### What I learned
The system keeps track of the active user, which is important when performing administrative or restricted actions.

---
## Question 3
Search the system for password wordlists that may be useful for security testing.
### Approach
I searched for common password wordlists stored in the system using a file searching command designed for quick lookup.
### Commands
- `locate wordlist` → searches system for files containing "wordlist"
- `locate rockyou` → finds common password dictionary files
### Output
##### STEP 1 : search for wordlists
