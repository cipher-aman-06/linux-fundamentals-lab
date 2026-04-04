
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
![[Pasted image 20260404062106.png]]
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
![[Pasted image 20260404064530.png]]
##### STEP 2 : launch tor browser
![[Pasted image 20260404064622.png]]
![[Pasted image 20260404064712.png]]
### Key Observations
Tor routes traffic through multiple encrypted relays.
Speed is slower due to multiple hops.
### What I learned
Anonymity networks trade speed for privacy.

---
## Question 3
Configure proxychains with Firefox and browse a website through proxy routing.
### Approach
Use proxychains tool to route browser traffic through chained proxies.
### Commands
- `proxychains` → route traffic through proxy
- `firefox` → launch browser
- `nano` → edit proxy configuration
### Output
##### STEP 1 : edit proxychains config
![[Pasted image 20260404071507.png]]
##### STEP 2 : launch firefox using proxychains
![[Pasted image 20260404071526.png]]
![[Pasted image 20260404071556.png]]
### Key Observations
Proxychains hides original IP address.
Multiple proxies increase anonymity.
### What I learned
Traffic obfuscation helps reduce traceability.

---
# Security Insights

1. Traceroute exposes network structure useful for reconnaissance.
2. Tor hides identity by routing traffic through anonymous nodes.
3. Proxychains masks IP by chaining multiple proxies.
---
