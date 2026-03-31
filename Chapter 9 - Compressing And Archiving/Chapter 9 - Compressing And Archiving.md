
---
## Question 1
Create three simple scripts and name them Linux4Hackers1, Linux4Hackers2, Linux4Hackers3
### Approach
I created three small bash scripts similar to previous chapter script and saved them with the required filenames.
### Commands
- `nano` → create script
- `echo` → display message
- `chmod +x` → make executable
### Output
##### STEP 1 : create first script
![[Pasted image 20260331052236.png]]
![[Pasted image 20260331052004.png]]
##### STEP 2 : create second script
![[Pasted image 20260331052246.png]]
![[Pasted image 20260331052036.png]]
##### STEP 3 : create third script
![[Pasted image 20260331052255.png]]
![[Pasted image 20260331052124.png]]
##### STEP 4 : make scripts executable
![[Pasted image 20260331052408.png]]
### Key Observations
Multiple scripts can be created and prepared for combining
### What I learned
Scripts can be grouped for packing or transfer.

---
## Question 2
Create tar archive named L4H from the three scripts
### Approach
I combined the three script files into one tar archive file.
### Commands
- `tar` → combine files
- `-c` → create archive
- `-f` → specify filename
### Output
##### STEP 1 : create tarball
![[Pasted image 20260331052643.png]]
##### STEP 2 : verify file
![[Pasted image 20260331052653.png]]
### Key Observations
Tar combines multiple files into single archive.
### What I learned
Tar simplifies file transfer and storage.

---
## Question 3
Compress L4H archive using gzip and then decompress
### Approach
I compressed the tar file using gzip and then restored it.
### Commands
- `gzip` → compress file
- `gunzip` → decompress file
### Output
##### STEP 1 : compress archive
![[Pasted image 20260331052846.png]]
##### STEP 2 : check compressed file
![[Pasted image 20260331052902.png]]
##### STEP 3 : decompress file
![[Pasted image 20260331052913.png]]
### Key Observations
Compression reduces file size.
### What I learned
gzip helps reduce storage and speeds transfer.

---
## Question 4
Compress L4H archive using bzip2 and compress command
### Approach
I used two different compression tools to compare results.
### Commands
- `bzip2` → stronger compression
- `compress` → traditional compression
### Output
##### STEP 1 : compress using bzip2
![[Pasted image 20260331053107.png]]
![[Pasted image 20260331053119.png]]
##### STEP 2 : decompress bzip2 file
![[Pasted image 20260331053129.png]]
![[Pasted image 20260331053142.png]]
##### STEP 3 : compress using compress tool
![[Pasted image 20260331053325.png]]
![[Pasted image 20260331053335.png]]
##### STEP 4 : decompress file
![[Pasted image 20260331053349.png]]
![[Pasted image 20260331053403.png]]
### Key Observations
Different tools produce different compression ratios.
### What I learned
Multiple compression methods exist for different use cases.

---
## Question 5
Create bit-by-bit copy of flash drive using dd command
### Approach
I used dd command to create an exact binary copy of a storage device.
### Commands
- `dd` → disk duplication tool
- `if` → input file/device
- `of` → output file
### Output
##### STEP 1 : identify drive
![[Pasted image 20260331053707.png]]
##### STEP 2 : create disk image
![[Pasted image 20260331055757.png]]
![[Pasted image 20260331055714.png]]
### Key Observations
dd copies entire disk including deleted data.
### What I learned
dd creates forensic-level disk images.

---
## Security Insights
1. Attackers often bundle tools into archives for stealth transfer.
2. Compressed files help hide malicious payloads.
3. gzip archives may contain hidden scripts or malware.
4. Strong compression helps evade detection systems.
5. dd can copy sensitive data including deleted files.

---
