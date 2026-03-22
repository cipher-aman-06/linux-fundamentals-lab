
---
## Question 1
Navigate to the directory that contains password wordlists used for security testing tools.
### Approach
I navigated to the directory that stores password wordlists commonly used in penetration testing tools.
### Commands
- `cd` → changes directory
- `pwd` → confirms current location
- `ls` → lists files inside directory
### Output
##### STEP 1 : Navigate to wordlists directory
![[Pasted image 20260323031855.png]]
##### STEP 2 : Verify current directory
![[Pasted image 20260323031909.png]]
##### STEP 3 : List available wordlists
![[Pasted image 20260323031943.png]]
### Key Observations
The directory contain multiple password lists used for brute-force and dictionary attacks.
### What I learned
Security tools often store wordlists in predefined directories that can be accessed through the terminal.

---
## Question 2
Display the contents of the password list file using a command-line tool.
### Approach
I used a command that prints file content directly in the terminal.
### Commands
- `cat` → displays file contents
### Output
##### STEP 1 : View contents of password list
![[Pasted image 20260323032700.png]]
### Key Observations
The file contains many commonly used passwords.
### What I learned
Wordlists contain possible passwords that attackers may test against login systems.

---
## Question 3
View the contains of the password list page by page using a command designed for large files.
### Approach
Since the file contains many entries, I used a command that allows scrolling output one screen at a time
### Commands
- `more` → displays file content page by page
### Output
##### STEP 1 : View file using more
![[Pasted image 20260323033644.png]]
### Key Observation
The output pauses after each screen, allowing controlled reading.
### What I learned
Some files are too large to read at once, so paging tools help navigate content efficiently.

---
## Question 4
Use a command that allows flexible navigation through a large file.
### Approach
I used a command that allows scrolling up and down within the file.
### Commands
- `less` → allows forward and backward navigation
### Output
##### STEP 1 : View file using less
![[Pasted image 20260323034805.png]]
### Key Observations
Unlike `more` , this command allows scrolling in both directions.
### What I learned
Efficient file viewing is important when analyzing logs or large datasets.

---
## Question 5
Display the password list with line numbers.
### Approach
I used a command that adds numbering to each line in the file.
##### Commands
- `nl` → adds line numbers to file output
### Output
##### STEP 1 : Show numbered lines
![[Pasted image 20260323035120.png]]
![[Pasted image 20260323035152.png]]
### Key Observations
Each password entry is assigned a line number.
### What I learned
Line numbering helps reference specific entries when analyzing large files.

---
## Question 6
Show only the last 20 entries from the password list.
### Approach
I used a command that displays the ending porting of a file.
### Commands
- `tail` → displays last lines of file
- `-20` → specifies number of lines
### Output
##### STEP 1 : Display last 20 passwords
![[Pasted image 20260323040016.png]]
### Key Observations
The command quickly shows the final entries without printing the whole file.
### What I learned
Viewing specific parts of files saves time when working with large datasets.

---
## Question 7
Filter the password lists to show only entries containing specific numbers.
### Approach
I combined two commands using a pipe to filter resul