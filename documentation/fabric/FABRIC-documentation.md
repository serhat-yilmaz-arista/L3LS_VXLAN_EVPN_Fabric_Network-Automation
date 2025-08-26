# FABRIC

## Table of Contents

- [Fabric Switches and Management IP](#fabric-switches-and-management-ip)
  - [Fabric Switches with inband Management IP](#fabric-switches-with-inband-management-ip)
- [Fabric Topology](#fabric-topology)
- [Fabric IP Allocation](#fabric-ip-allocation)
  - [Fabric Point-To-Point Links](#fabric-point-to-point-links)
  - [Point-To-Point Links Node Allocation](#point-to-point-links-node-allocation)
  - [Loopback Interfaces (BGP EVPN Peering)](#loopback-interfaces-bgp-evpn-peering)
  - [Loopback0 Interfaces Node Allocation](#loopback0-interfaces-node-allocation)
  - [VTEP Loopback VXLAN Tunnel Source Interfaces (VTEPs Only)](#vtep-loopback-vxlan-tunnel-source-interfaces-vteps-only)
  - [VTEP Loopback Node allocation](#vtep-loopback-node-allocation)

## Fabric Switches and Management IP

| POD | Type | Node | Management IP | Platform | Provisioned in CloudVision | Serial Number |
| --- | ---- | ---- | ------------- | -------- | -------------------------- | ------------- |
| FABRIC | l3leaf | Leaf1 | 172.20.20.69/24 | cEOS-LAB | Provisioned | - |
| FABRIC | l3leaf | Leaf2 | 172.20.20.65/24 | cEOS-LAB | Provisioned | - |
| FABRIC | l3leaf | Leaf3 | 172.20.20.73/24 | cEOS-LAB | Provisioned | - |
| FABRIC | l3leaf | Leaf4 | 172.20.20.68/24 | cEOS-LAB | Provisioned | - |
| FABRIC | l3leaf | Leaf5 | 172.20.20.71/24 | cEOS-LAB | Provisioned | - |
| FABRIC | l3leaf | Leaf6 | 172.20.20.63/24 | cEOS-LAB | Provisioned | - |
| FABRIC | spine | Spine1 | 172.20.20.72/24 | cEOS-LAB | Provisioned | - |
| FABRIC | spine | Spine2 | 172.20.20.66/24 | cEOS-LAB | Provisioned | - |

> Provision status is based on Ansible inventory declaration and do not represent real status from CloudVision.

### Fabric Switches with inband Management IP

| POD | Type | Node | Management IP | Inband Interface |
| --- | ---- | ---- | ------------- | ---------------- |

## Fabric Topology

| Type | Node | Node Interface | Peer Type | Peer Node | Peer Interface |
| ---- | ---- | -------------- | --------- | ----------| -------------- |
| l3leaf | Leaf1 | Ethernet1 | spine | Spine1 | Ethernet1 |
| l3leaf | Leaf1 | Ethernet2 | spine | Spine2 | Ethernet1 |
| l3leaf | Leaf1 | Ethernet3 | mlag_peer | Leaf2 | Ethernet3 |
| l3leaf | Leaf1 | Ethernet4 | mlag_peer | Leaf2 | Ethernet4 |
| l3leaf | Leaf2 | Ethernet1 | spine | Spine1 | Ethernet2 |
| l3leaf | Leaf2 | Ethernet2 | spine | Spine2 | Ethernet2 |
| l3leaf | Leaf3 | Ethernet1 | spine | Spine1 | Ethernet3 |
| l3leaf | Leaf3 | Ethernet2 | spine | Spine2 | Ethernet3 |
| l3leaf | Leaf3 | Ethernet3 | mlag_peer | Leaf4 | Ethernet3 |
| l3leaf | Leaf3 | Ethernet4 | mlag_peer | Leaf4 | Ethernet4 |
| l3leaf | Leaf4 | Ethernet1 | spine | Spine1 | Ethernet4 |
| l3leaf | Leaf4 | Ethernet2 | spine | Spine2 | Ethernet4 |
| l3leaf | Leaf5 | Ethernet1 | spine | Spine1 | Ethernet5 |
| l3leaf | Leaf5 | Ethernet2 | spine | Spine2 | Ethernet5 |
| l3leaf | Leaf5 | Ethernet3 | mlag_peer | Leaf6 | Ethernet3 |
| l3leaf | Leaf5 | Ethernet4 | mlag_peer | Leaf6 | Ethernet4 |
| l3leaf | Leaf6 | Ethernet1 | spine | Spine1 | Ethernet6 |
| l3leaf | Leaf6 | Ethernet2 | spine | Spine2 | Ethernet6 |

## Fabric IP Allocation

### Fabric Point-To-Point Links

| Uplink IPv4 Pool | Available Addresses | Assigned addresses | Assigned Address % |
| ---------------- | ------------------- | ------------------ | ------------------ |
| 10.255.255.0/26 | 64 | 24 | 37.5 % |

### Point-To-Point Links Node Allocation

| Node | Node Interface | Node IP Address | Peer Node | Peer Interface | Peer IP Address |
| ---- | -------------- | --------------- | --------- | -------------- | --------------- |
| Leaf1 | Ethernet1 | 10.255.255.1/31 | Spine1 | Ethernet1 | 10.255.255.0/31 |
| Leaf1 | Ethernet2 | 10.255.255.3/31 | Spine2 | Ethernet1 | 10.255.255.2/31 |
| Leaf2 | Ethernet1 | 10.255.255.5/31 | Spine1 | Ethernet2 | 10.255.255.4/31 |
| Leaf2 | Ethernet2 | 10.255.255.7/31 | Spine2 | Ethernet2 | 10.255.255.6/31 |
| Leaf3 | Ethernet1 | 10.255.255.9/31 | Spine1 | Ethernet3 | 10.255.255.8/31 |
| Leaf3 | Ethernet2 | 10.255.255.11/31 | Spine2 | Ethernet3 | 10.255.255.10/31 |
| Leaf4 | Ethernet1 | 10.255.255.13/31 | Spine1 | Ethernet4 | 10.255.255.12/31 |
| Leaf4 | Ethernet2 | 10.255.255.15/31 | Spine2 | Ethernet4 | 10.255.255.14/31 |
| Leaf5 | Ethernet1 | 10.255.255.17/31 | Spine1 | Ethernet5 | 10.255.255.16/31 |
| Leaf5 | Ethernet2 | 10.255.255.19/31 | Spine2 | Ethernet5 | 10.255.255.18/31 |
| Leaf6 | Ethernet1 | 10.255.255.21/31 | Spine1 | Ethernet6 | 10.255.255.20/31 |
| Leaf6 | Ethernet2 | 10.255.255.23/31 | Spine2 | Ethernet6 | 10.255.255.22/31 |

### Loopback Interfaces (BGP EVPN Peering)

| Loopback Pool | Available Addresses | Assigned addresses | Assigned Address % |
| ------------- | ------------------- | ------------------ | ------------------ |
| 10.255.0.0/27 | 32 | 8 | 25.0 % |

### Loopback0 Interfaces Node Allocation

| POD | Node | Loopback0 |
| --- | ---- | --------- |
| FABRIC | Leaf1 | 10.255.0.3/32 |
| FABRIC | Leaf2 | 10.255.0.4/32 |
| FABRIC | Leaf3 | 10.255.0.5/32 |
| FABRIC | Leaf4 | 10.255.0.6/32 |
| FABRIC | Leaf5 | 10.255.0.7/32 |
| FABRIC | Leaf6 | 10.255.0.8/32 |
| FABRIC | Spine1 | 10.255.0.1/32 |
| FABRIC | Spine2 | 10.255.0.2/32 |

### VTEP Loopback VXLAN Tunnel Source Interfaces (VTEPs Only)

| VTEP Loopback Pool | Available Addresses | Assigned addresses | Assigned Address % |
| ------------------ | ------------------- | ------------------ | ------------------ |
| 192.168.1.0/27 | 32 | 4 | 12.5 % |
| 192.168.2.0/27 | 32 | 2 | 6.25 % |

### VTEP Loopback Node allocation

| POD | Node | Loopback1 |
| --- | ---- | --------- |
| FABRIC | Leaf1 | 192.168.1.3/32 |
| FABRIC | Leaf2 | 192.168.1.3/32 |
| FABRIC | Leaf3 | 192.168.1.5/32 |
| FABRIC | Leaf4 | 192.168.1.5/32 |
| FABRIC | Leaf5 | 192.168.2.7/32 |
| FABRIC | Leaf6 | 192.168.2.7/32 |
