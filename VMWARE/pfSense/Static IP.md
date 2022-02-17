# STATIC IP:
- go to [[PfSense]]: 10.1.0.1 go to `Services` -> `DHCP Server`
- Look right and click the graph icon also called `Related status` (edited) 
- There is a section called Leases where all your VMs should be on the right side click the left plus called `Add static mapping` (edited) 
- Give it an `IP Address` that must be outside the dns pool most likely between 10.1.0.`11-49`
- Host name should be set already but otherwise set it with the machine name
- Press save and apply changes

NOTE DO NOT FORGET TO RESTART VM AFTER ASSIGNING STATIC IP