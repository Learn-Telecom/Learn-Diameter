---
coverY: 0
---

# Diameter Peers

Nodes with a direct TCP or SCTP transport connection are Peers.&#x20;

• A node SHOULD have a connection with at least two peers per realm (primary and secondary).&#x20;

• Peers may be statically configured or dynamically discovered&#x20;

• Static configuration requires: - either the IP address, or - the FQDN (DNS can then resolve FQDN into IP-address)&#x20;

• Dynamic discovery based on: - DNS procedures using NAPTR and/or SRV queries&#x20;

A new Peer creates an entry in the&#x20;

\- Peer Table, and&#x20;

\- Routing Table (for other realms)&#x20;

Entries created via DNS MUST be refreshed periodically.&#x20;

When no transport connection exists with a peer, an attempt to connect SHOULD be made periodically (recommended every 30 s).
