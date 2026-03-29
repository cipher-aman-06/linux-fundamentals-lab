
---
## Question 1
Display all environment variables using the more command
### Approach
I listed all environment variables and piped the output into the more command to view them page by page.
### Commands
- `env` → shows environment variables
- `printenv` → alternative command
- `more` → displays output page by page
### Output
##### STEP 1 : view environment variables
![[Pasted image 20260329193335.png]]
### Key Observations
Environment variables store system configuration values such as :
- USER
- HOME
- PATH
- SHELL
### What I learned
Environment variables store important system configuration information.

---
## Question 2
Display the HOSTNAME variable using echo
### Approach
I used the echo command to print the value stored in the HOSTNAME variable.
### Commands
- `echo` → prints variable value
- `$HOSTNAME` → stores system hostname
### Output
##### STEP 1 : display hostname variable
![[Pasted image 20260329193639.png]]
### Key Observations
HOSTNAME identifies the system name on the network.
### What I learned
Environment variables can be accessed using the `$` symbol.

---
## Question 3
Modify the PS1 variable to change forward slash to backslash
### Approach
I modified the PS1 environment variable to change the shell prompt appearance.
### Commands
- `PS1` → controls terminal prompt appearance.
### Output
##### STEP 1 : modify PS1 prompt
![[Pasted image 20260329194019.png]]
### Key Observations
Changing PS1 alters how the terminal prompt is displayed.
### What I learned
PS1 variable customizes command line appearance.

---
## Question 4
Create a new variable named MYNEWVARIABLE and assign a value
### Approach
I created a custom environment variable and assigned my name as its value.
### Commands
- variable format : `VARIABLE_NAME=value` 
### Output
##### STEP 1 : create variable
![[Pasted image 20260329201330.png]]
### Key Observations
Variables are created without spaces around the equals sign.
### What I learned
Custom variables can store user-defined values.

---
## Question 5
Display the value stored in MYNEWVARIABLE
### Approach
I used echo command to display the stored value.
### Commands
- `$VARIABLE_NAME` → retrieves stored value
### Output
##### STEP 1 : display variable value
![[Pasted image 20260329201343.png]]
### Key Observations
Echo prints the stored variable value.
### What I learned
Variables store reusable values accessible throughout the session.

---
## Question 6
Export MYNEWVARIABLE so it is available globally
### Approach
I used the export command to make the variable available across different shell environments.
### Commands
-  `export` → makes variable available globally
### Output
##### STEP 1 : export variable
![[Pasted image 20260329202441.png]]
##### STEP 2 : verify export
![[Pasted image 20260329202507.png]]
### Key Observations
Exported variables can be accessed by child processes.

### What I learned
Export allows variables to persist across different shell sessions.

---
## Question 7
Display the PATH variable
### Approach
I used echo to display directories stored in the PATH variable.
### Commands
-  `PATH` → list of executable directories
### Output
##### STEP 1 : display PATH variable
### Key Observations
PATH contains directories separated by colon (:)
`/usr/bin:/bon:/usr/sbin`
### What I learned
PATH determines where the system looks for executable files.

---
## Question 8
Add home directory to PATH variable
