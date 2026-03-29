
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
