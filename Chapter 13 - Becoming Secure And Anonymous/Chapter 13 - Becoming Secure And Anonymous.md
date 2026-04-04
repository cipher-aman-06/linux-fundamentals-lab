
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
##### STEP 2 : launch firefox using proxychains
### Key Observations
Proxychains hides original IP address.
Multiple proxies increase anonymity.
### What I learned
Traffic obfuscation helps reduce traceability.

---
## Question 4
Research VPN providers and test one trial service.
### Approach
Select VPN provider, install client, and connect to secure server.
### Commands
- `openvpn` → VPN client
- `wget` → download config
- `systemctl` → manage service
### Output
##### STEP 1 : install vpn client
##### STEP 2 : connect vpn
### Key Observations
VPN encrypts traffic between user and VPN server.
IP address changes after connection.
### What I learned
VPN protects network traffic from monitoring.

---
## Question 5
Create ProtonMail account and send encrypted email message.
### Approach
Register secure email account and send message using encrypted platform.
### Commands
- `firefox` →open website
- `https` → secure wen communication
### Output
##### STEP 1: open protonmail website
##### STEP 2 : send secure email
### Key Observations
ProtonMail provides end-to-end encryption.  
Encrypted emails protect message confidentiality.
## What I Learned
Secure email reduces risk of interception.

---
# Security Insights

1. Traceroute exposes network structure useful for reconnaissance.
2. Tor hides identity by routing traffic through anonymous nodes.
3. Proxychains masks IP by chaining multiple proxies.
4. VPN encrypts traffic to prevent ISP surveillance.
5. Encrypted email protects communication privacy.
---
