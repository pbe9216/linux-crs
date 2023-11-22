## Linux firewalling

### Host firewalling nftables
In this task you will protect srv1 host.
- Install nftables
- Prepare the ruleset
- Look for current services listening
- Look for established connections
- Display for process information 
- Allow SSH
- Allow DNS
- Allow established connections
- Allow ICMP
- Allow traceroute
- Restrict outbound traffic (APT, DNS, established)
- How does this interact with the DHCP server?
- Check ruleset and if rules are matched
- Set all base policies to drop
- Observe what happens

### Firewalld implementation and connection tracking

On firewall hosts fw1 and fw2
- install firewalld
- configure 2 zones according (you can try subdividing the ports)
- allow icmp and tcp 22 between the two zones
- deploy connection tracking between the two firewall nodes to ensure failover
- deploy a fhrp between the two nodes to have unique gateway for the hosts
- route some traffic over that firewall
- observe traffic matched by firewalld
- test a failover
- analyze the results
