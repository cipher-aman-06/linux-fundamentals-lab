
---
## Question 1
Configure the MySQLscanner script to execute automatically every Wednesday at 3PM.
### Approach
Use cron scheduler to run script weekly at specified day and time.
### Commands
- `crontab -e` → edit cron jobs
- `0 15 * * 3` → schedule format (3 PM Wednesday )
### Output
##### STEP 1 : open cron editor
![[Pasted image 20260405160622.png]]
##### STEP 2 : add scheduled task
![[Pasted image 20260405160342.png]]
![[Pasted image 20260405160642.png]]
### Key Observations
Cron uses 24-hour time format.
Day value 3 represents Wednesday.
### What I learned
Cron enables precise automation of security scripts.

---
## Question 2
Schedule the MySQLscanner script to execute on the 10th day of April, June, and August.
### Approach
Define cron job specifying day of month and selected months.
### Commands
