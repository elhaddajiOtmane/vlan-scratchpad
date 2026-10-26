# VLAN scratchpad

A tiny two-VLAN topology for thinking through access ports, trunk links, and why packets sometimes reach a gateway but not another subnet.

The IP plan is a sample design, not an export from a live network. I haven't included a Packet Tracer `.pkt` file—those need to be created in Packet Tracer itself.

## Topology
![Example VLAN topology](assets/vlan-topology.svg)

## Addresses
- VLAN 10 — 192.168.10.0/24
- VLAN 20 — 192.168.20.0/24
- Router subinterfaces can provide inter-VLAN routing if supported by the chosen model.

## Things to experiment with
Assign the wrong VLAN to a switch port, inspect `show vlan brief` / `show interfaces trunk`, and repair the mismatch in a private simulator.

## References
[Cisco Packet Tracer](https://www.netacad.com/cisco-packet-tracer) · [Network switch photos](https://commons.wikimedia.org/wiki/Special:MediaSearch?type=image&search=network%20switch)
