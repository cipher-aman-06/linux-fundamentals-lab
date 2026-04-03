
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
Network paths reev