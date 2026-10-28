
# Details
## Devices
|Device|Qty.|Suggested model|Role|
|------|----|---------------|----|
|ISP routers|2|Cisco 2911 or available equivalent|Simulated Internet providers| 
Enterprise edge routers|2|Cisco 2911 or available equivalent|Enterprise WAN connectivity|
Core multilayer switches|2|Cisco 3560|Internal routing and redundancy|
Access switches|4|Cisco 2960|Connect users and servers|
PCs|8–12|PC-PT|Department endpoints|
Servers	2|Server-PT|DNS, HTTP and other services|
External test server|1|Server-PT|Simulated public Internet destination|

## IP Assignment
|Network purpose|Subnet|Devices|
|---------------|------|-------|
|ISP 1 ↔ Edge Router 1|203.0.113.0/30|ISP 1, Edge R1|
|ISP 2 ↔ Edge Router 2|198.51.100.0/30|ISP 2, Edge R2|
|Edge R1 ↔ Core SW1|10.255.0.0/30|R1, MLS1|
|Edge R1 ↔ Core SW2|10.255.0.4/30|R1, MLS2|
|Edge R2 ↔ Core SW1|10.255.0.8/30|R2, MLS1|
|Edge R2 ↔ Core SW2|10.255.0.12/30|R2, MLS2|

## VLAN plan
|VLAN|Department|Subnet|Default gateway|
|----|----------|------|---------------|
|10|Administration|10.10.10.0/24|10.10.10.1|
|20|Accounts|10.10.20.0/24|10.10.20.1|
|30|IT|10.10.30.0/24|10.10.30.1|
|40|Servers|10.10.40.0/24|10.10.40.1|
|50|Guest|Wi-Fi|10.10.50.0/24|10.10.50.1|
|99|Network management|10.10.99.0/24|10.10.99.1|

# Diagram
![initial](./image/Screenshot%202026-10-27%20164304.png)
