## Linux networking lab 2 

- Check IPv6 configured on your interfaces? Which ones is there?
- Configure GUA IPv6 addresses on VyOS VM (2001:DB8:0:1::/64). Enable RA prefix advertisement.
- What is the outcome of this change? What is the address of the end host?
- Enable privacy extensions for SLAAC
- Observe the outcome after bouncing the interface
- Configure all the VMs like that. 
- Check the neighbor discovery table
- On srv1 install the Kea DHCP service
- Configure a DHCP pool
- Observe DHCP traffic using tcpdump
- Configure a DHCP relay on the router
- Test and observe a client request behind the relay

Bonus
- Install the DNS server role on srv1
- Configure a local zone testlab.local and register somes names
- Test and observe name resolution with tcpdump
