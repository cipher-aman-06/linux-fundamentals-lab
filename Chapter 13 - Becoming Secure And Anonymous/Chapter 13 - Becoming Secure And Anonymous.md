
---
## Question 1
Trace the network path to a website and count how many intermediate routers are involved.
### Approach
Use network diagnostic tool to view packet route and identify hop count.
### Commands
- `traceroute` → shows network path
- `traceroute domain` → displays hop sequence
### Output
##### STEP 1 : run traceroute
### Key Observations
Each hop represents a router between source and destination.
Higher hops may indicate longer routing path.
### What I learned
Network paths reveal infrastructure between user and website.

---
## Question 2
Install Tor browser and compare browsing speed with normal browsing.
### Approach
Install Tor package and open browser to test anonymous browsing performance.
### Commands
- `apt install` → install software
- `torbrowser-launcher` → launch tor browser
### Output
##### STEP 1 : install tor browser
##### STEP 2 : launch tor browser
### Key Observations
Tor routes traffic through multiple encrypted relays.
Speed is slower due to multiple hops.
### What I learned
Anonymity networks trade speed for privay.
