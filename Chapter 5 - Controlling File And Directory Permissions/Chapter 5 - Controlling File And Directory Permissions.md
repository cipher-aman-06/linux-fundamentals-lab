
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
## Question 2
Grant execute permission to a file using both numeric and symbolic methods
### Approach
I selected a file without execute permission and modified permissions using the `chmod` command. I applied both, numeric (777) and symbolic (u+x) permission methods.
### Commands
- `chmod` → change file permissions
- numeric method → uses numbers
- symbolic method → uses letters
Permission values :
- 4 → read
- 2 → write
- 1 → execute
### Output
##### STEP 1 : Create test file
![[Pasted image 20260329015027.png]]
##### STEP 2 : Check permissions
![[Pasted image 20260329015103.png]]
##### STEP 3 : Give execute permission using numeric method
![[Pasted image 20260329015141.png]]
##### STEP 4 : Give execute permission using symbolic method
![[Pasted image 20260329015232.png]]
##### STEP 5 : Verify permission change
![[Pasted image 20260329015306.png]]
### Key Observation
Permission changes reflect immediately in the file listing
`-rwxrwxrwx`
### What I learned
Permissions can be modified numerically or symbolically to control file access.

---
## Question 3
Change file ownership using chown command
### Approach
I selected a file and changed its owner using the chown command.
### Commands
- `chown` → change file ownership
- syntax : `sudo chown user:group filename`
### Output
##### STEP 1 : Create new file
