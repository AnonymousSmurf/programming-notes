# ADD FIREWALL RULE
## Example(SSH): 
- go to [[PfSense]]: 10.1.0.1
- go to `Firewall` -> `NAT` 
- `Destination port` at the left `Custom` set `22` right `Custom` set `22` you can change this depending on what port you want
-  `Redirect target IP` set `Address` to the VMs IP
- `Redirect target port` set `Custom` to `22`
- `Description` set this to a clear description of what the rule does
- Save the change and apply them 
- NOTE: you most likely have to restart your VM
