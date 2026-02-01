# Assumptions

- Each station is represented by a single router, and switches are used to connect end devices (PCs, servers, printers).
- Central acts as the hub station. Town Hall and Wynyard connect directly to Central, while Burwood and Parramatta connect through Redfern.
- Central hosts the DHCP, DNS, and Web servers. Parramatta hosts the Email server.
- WAN connectivity uses serial links; LAN connectivity uses Fast Ethernet.
- Redundancy is provided using two serial paths for failover:
  - Primary: Wynyard → Central
  - Backup: Wynyard → Town Hall → Central
- Email accounts are registered using station names only, and all stations can exchange emails.
