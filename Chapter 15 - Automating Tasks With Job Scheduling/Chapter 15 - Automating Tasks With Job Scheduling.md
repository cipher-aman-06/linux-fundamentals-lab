
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
