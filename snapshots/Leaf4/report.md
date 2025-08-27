# Leaf4 Commands Output

## Table of Contents

- [show version](#show-version)
- [show running-config](#show-running-config)
- [show lldp neighbors](#show-lldp-neighbors)
- [show interfaces description](#show-interfaces-description)
- [show bgp summary](#show-bgp-summary)
- [show bgp evpn summary](#show-bgp-evpn-summary)
- [show bgp evpn route-type mac-ip](#show-bgp-evpn-route-type-mac-ip)
- [show bgp evpn route-type imet](#show-bgp-evpn-route-type-imet)
- [show bgp evpn route-type ip-prefix](#show-bgp-evpn-route-type-ip-prefix)
- [show vxlan vni](#show-vxlan-vni)
- [show interfaces vxlan1](#show-interfaces-vxlan1)
- [show ip route](#show-ip-route)
- [show ip bgp](#show-ip-bgp)
- [show arp](#show-arp)
## show arp

```
Address         Age (sec)  Hardware Addr   Interface
10.255.255.12     0:00:17  aac1.abb4.fad5  Ethernet1
10.255.255.14     0:00:29  aac1.abee.1c07  Ethernet2
10.255.1.100      0:00:22  001c.eaae.13b2  Vlan4093, Port-Channel3
10.255.1.68       0:00:00  001c.eaae.13b2  Vlan4094, Port-Channel3
172.20.20.1       0:00:00  9a5f.f8e6.7bd6  Management0
```
## show bgp evpn route-type imet

```
BGP routing table information for VRF default
Router identifier 10.255.0.6, local AS number 65002
Route status codes: * - valid, > - active, S - Stale, E - ECMP head, e - ECMP
                    c - Contributing to ECMP, % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
 * >Ec    RD: 10.255.0.3:10011 imet 192.168.1.3
                                 192.168.1.3           -       100     0       65100 65001 i
 *  ec    RD: 10.255.0.3:10011 imet 192.168.1.3
                                 192.168.1.3           -       100     0       65100 65001 i
 * >Ec    RD: 10.255.0.3:10012 imet 192.168.1.3
                                 192.168.1.3           -       100     0       65100 65001 i
 *  ec    RD: 10.255.0.3:10012 imet 192.168.1.3
                                 192.168.1.3           -       100     0       65100 65001 i
 * >Ec    RD: 10.255.0.4:10011 imet 192.168.1.3
                                 192.168.1.3           -       100     0       65100 65001 i
 *  ec    RD: 10.255.0.4:10011 imet 192.168.1.3
                                 192.168.1.3           -       100     0       65100 65001 i
 * >Ec    RD: 10.255.0.4:10012 imet 192.168.1.3
                                 192.168.1.3           -       100     0       65100 65001 i
 *  ec    RD: 10.255.0.4:10012 imet 192.168.1.3
                                 192.168.1.3           -       100     0       65100 65001 i
 * >      RD: 10.255.0.6:10021 imet 192.168.1.5
                                 -                     -       -       0       i
 * >      RD: 10.255.0.6:10022 imet 192.168.1.5
                                 -                     -       -       0       i
 * >Ec    RD: 10.255.0.7:10031 imet 192.168.1.7
                                 192.168.1.7           -       100     0       65100 65005 i
 *  ec    RD: 10.255.0.7:10031 imet 192.168.1.7
                                 192.168.1.7           -       100     0       65100 65005 i
 * >Ec    RD: 10.255.0.7:10032 imet 192.168.1.7
                                 192.168.1.7           -       100     0       65100 65005 i
 *  ec    RD: 10.255.0.7:10032 imet 192.168.1.7
                                 192.168.1.7           -       100     0       65100 65005 i
 * >Ec    RD: 10.255.0.8:10031 imet 192.168.1.8
                                 192.168.1.8           -       100     0       65100 65006 i
 *  ec    RD: 10.255.0.8:10031 imet 192.168.1.8
                                 192.168.1.8           -       100     0       65100 65006 i
 * >Ec    RD: 10.255.0.8:10032 imet 192.168.1.8
                                 192.168.1.8           -       100     0       65100 65006 i
 *  ec    RD: 10.255.0.8:10032 imet 192.168.1.8
                                 192.168.1.8           -       100     0       65100 65006 i
```
## show bgp evpn route-type ip-prefix

```
BGP routing table information for VRF default
Router identifier 10.255.0.6, local AS number 65002
Route status codes: * - valid, > - active, S - Stale, E - ECMP head, e - ECMP
                    c - Contributing to ECMP, % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
 * >Ec    RD: 10.255.0.3:10 ip-prefix 10.10.11.0/24
                                 192.168.1.3           -       100     0       65100 65001 i
 *  ec    RD: 10.255.0.3:10 ip-prefix 10.10.11.0/24
                                 192.168.1.3           -       100     0       65100 65001 i
 * >Ec    RD: 10.255.0.4:10 ip-prefix 10.10.11.0/24
                                 192.168.1.3           -       100     0       65100 65001 i
 *  ec    RD: 10.255.0.4:10 ip-prefix 10.10.11.0/24
                                 192.168.1.3           -       100     0       65100 65001 i
 * >      RD: 10.255.0.6:10 ip-prefix 10.10.11.0/24
                                 -                     -       100     0       65100 65001 ?
 * >Ec    RD: 10.255.0.3:10 ip-prefix 10.10.12.0/24
                                 192.168.1.3           -       100     0       65100 65001 i
 *  ec    RD: 10.255.0.3:10 ip-prefix 10.10.12.0/24
                                 192.168.1.3           -       100     0       65100 65001 i
 * >Ec    RD: 10.255.0.4:10 ip-prefix 10.10.12.0/24
                                 192.168.1.3           -       100     0       65100 65001 i
 *  ec    RD: 10.255.0.4:10 ip-prefix 10.10.12.0/24
                                 192.168.1.3           -       100     0       65100 65001 i
 * >      RD: 10.255.0.6:10 ip-prefix 10.10.12.0/24
                                 -                     -       100     0       65100 65001 ?
 * >      RD: 10.255.0.6:10 ip-prefix 10.10.21.0/24
                                 -                     -       -       0       i
 *        RD: 10.255.0.6:10 ip-prefix 10.10.21.0/24
                                 -                     -       100     0       ?
 * >      RD: 10.255.0.6:10 ip-prefix 10.10.22.0/24
                                 -                     -       -       0       i
 *        RD: 10.255.0.6:10 ip-prefix 10.10.22.0/24
                                 -                     -       100     0       ?
 * >      RD: 10.255.0.6:10 ip-prefix 10.10.31.0/24
                                 -                     -       100     0       65100 65006 ?
 * >Ec    RD: 10.255.0.7:10 ip-prefix 10.10.31.0/24
                                 192.168.1.7           -       100     0       65100 65005 i
 *  ec    RD: 10.255.0.7:10 ip-prefix 10.10.31.0/24
                                 192.168.1.7           -       100     0       65100 65005 i
 * >Ec    RD: 10.255.0.8:10 ip-prefix 10.10.31.0/24
                                 192.168.1.8           -       100     0       65100 65006 i
 *  ec    RD: 10.255.0.8:10 ip-prefix 10.10.31.0/24
                                 192.168.1.8           -       100     0       65100 65006 i
 * >      RD: 10.255.0.6:10 ip-prefix 10.10.32.0/24
                                 -                     -       100     0       65100 65006 ?
 * >Ec    RD: 10.255.0.7:10 ip-prefix 10.10.32.0/24
                                 192.168.1.7           -       100     0       65100 65005 i
 *  ec    RD: 10.255.0.7:10 ip-prefix 10.10.32.0/24
                                 192.168.1.7           -       100     0       65100 65005 i
 * >Ec    RD: 10.255.0.8:10 ip-prefix 10.10.32.0/24
                                 192.168.1.8           -       100     0       65100 65006 i
 *  ec    RD: 10.255.0.8:10 ip-prefix 10.10.32.0/24
                                 192.168.1.8           -       100     0       65100 65006 i
```
## show bgp evpn route-type mac-ip

```
BGP routing table information for VRF default
Router identifier 10.255.0.6, local AS number 65002
Route status codes: * - valid, > - active, S - Stale, E - ECMP head, e - ECMP
                    c - Contributing to ECMP, % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
```
## show bgp evpn summary

```
BGP summary information for VRF default
Router identifier 10.255.0.6, local AS number 65002
Neighbor Status Codes: m - Under maintenance
  Description              Neighbor   V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc PfxAdv
  Spine1_Loopback0         10.255.0.1 4 65100            111       110    0    0 01:17:34 Estab   16     16     12
  Spine2_Loopback0         10.255.0.2 4 65100            108       112    0    0 01:17:34 Estab   16     16     20
```
## show bgp summary

```
BGP summary information for VRF default
Router identifier 10.255.0.6, local AS number 65002
Neighbor               AS Session State AFI/SAFI                AFI/SAFI State   NLRI Rcd   NLRI Acc   NLRI Adv
------------- ----------- ------------- ----------------------- -------------- ---------- ---------- ----------
10.255.0.1          65100 Established   L2VPN EVPN              Negotiated             16         16         12
10.255.0.2          65100 Established   L2VPN EVPN              Negotiated             16         16         20
10.255.1.100        65002 Established   IPv4 Unicast            Negotiated             11         11         11
10.255.255.12       65100 Established   IPv4 Unicast            Negotiated              8          8          6
10.255.255.14       65100 Established   IPv4 Unicast            Negotiated              8          8          9
```
## show interfaces description

```
Interface                      Status         Protocol           Description
Et1                            up             up                 P2P_Spine1_Ethernet4
Et2                            up             up                 P2P_Spine2_Ethernet4
Et3                            up             up                 MLAG_Leaf3_Ethernet3
Et4                            up             up                 MLAG_Leaf3_Ethernet4
Et5                            up             up                 SERVER_Host-C_Ethernet2
Et6                            up             up                 SERVER_Host-D_Ethernet2
Lo0                            up             up                 ROUTER_ID
Lo1                            up             up                 VXLAN_TUNNEL_SOURCE
Ma0                            up             up                 OOB_MANAGEMENT
Po3                            up             up                 MLAG_Leaf3_Port-Channel3
Po5                            down           lowerlayerdown     MLAG_PortChannel
Po6                            down           lowerlayerdown     MLAG_PortChannel
Vl21                           up             up                 VRF_A_VLAN_21
Vl22                           up             up                 VRF_A_VLAN_22
Vl3009                         up             up                 MLAG_L3_VRF_VRF_A
Vl4093                         up             up                 MLAG_L3
Vl4094                         up             up                 MLAG
Vl4097                         up             up                 
Vx1                            up             up                 Leaf4_VTEP
```
## show interfaces vxlan1

```
Vxlan1 is up, line protocol is up (connected)
  Hardware is Vxlan
  Description: Leaf4_VTEP
  Source interface is Loopback1 and is active with 192.168.1.5
  Listening on UDP port 4789
  Replication/Flood Mode is headend with Flood List Source: EVPN
  Remote MAC learning via EVPN
  VNI mapping to VLANs
  Static VLAN to VNI mapping is 
    [21, 10021]       [22, 10022]      
  Dynamic VLAN to VNI mapping for 'evpn' is
    [4097, 10]       
  Note: All Dynamic VLANs used by VCS are internal VLANs.
        Use 'show vxlan vni' for details.
  Static VRF to VNI mapping is 
   [VRF_A, 10]
  MLAG Shared Router MAC is 021c.eaae.13b2
```
## show ip bgp

```
BGP routing table information for VRF default
Router identifier 10.255.0.6, local AS number 65002
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast, q - Pending FIB install
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
RPKI Origin Validation codes: V - valid, I - invalid, U - unknown
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  AIGP       LocPref Weight  Path
 * >      10.255.0.1/32          10.255.255.12         0       -          100     0       65100 i
 *        10.255.0.1/32          10.255.1.100          0       -          100     0       65100 ?
 * >      10.255.0.2/32          10.255.255.14         0       -          100     0       65100 i
 *        10.255.0.2/32          10.255.1.100          0       -          100     0       65100 ?
 * >Ec    10.255.0.3/32          10.255.255.12         0       -          100     0       65100 65001 i
 *  ec    10.255.0.3/32          10.255.255.14         0       -          100     0       65100 65001 i
 *        10.255.0.3/32          10.255.1.100          0       -          100     0       65100 65001 ?
 * >Ec    10.255.0.4/32          10.255.255.12         0       -          100     0       65100 65001 i
 *  ec    10.255.0.4/32          10.255.255.14         0       -          100     0       65100 65001 i
 *        10.255.0.4/32          10.255.1.100          0       -          100     0       65100 65001 ?
 * >      10.255.0.5/32          10.255.1.100          0       -          100     0       ?
 * >      10.255.0.6/32          -                     -       -          -       0       i
 * >Ec    10.255.0.7/32          10.255.255.14         0       -          100     0       65100 65005 i
 *  ec    10.255.0.7/32          10.255.255.12         0       -          100     0       65100 65005 i
 *        10.255.0.7/32          10.255.1.100          0       -          100     0       65100 65005 ?
 * >Ec    10.255.0.8/32          10.255.255.12         0       -          100     0       65100 65006 i
 *  ec    10.255.0.8/32          10.255.255.14         0       -          100     0       65100 65006 i
 *        10.255.0.8/32          10.255.1.100          0       -          100     0       65100 65006 ?
 * >Ec    192.168.1.3/32         10.255.255.12         0       -          100     0       65100 65001 i
 *  ec    192.168.1.3/32         10.255.255.14         0       -          100     0       65100 65001 i
 *        192.168.1.3/32         10.255.1.100          0       -          100     0       65100 65001 ?
 * >      192.168.1.5/32         -                     -       -          -       0       i
 *        192.168.1.5/32         10.255.1.100          0       -          100     0       ?
 * >Ec    192.168.1.7/32         10.255.255.14         0       -          100     0       65100 65005 i
 *  ec    192.168.1.7/32         10.255.255.12         0       -          100     0       65100 65005 i
 *        192.168.1.7/32         10.255.1.100          0       -          100     0       65100 65005 ?
 * >Ec    192.168.1.8/32         10.255.255.12         0       -          100     0       65100 65006 i
 *  ec    192.168.1.8/32         10.255.255.14         0       -          100     0       65100 65006 i
 *        192.168.1.8/32         10.255.1.100          0       -          100     0       65100 65006 ?
```
## show ip route

```
VRF: default
Source Codes:
       C - connected, S - static, K - kernel,
       O - OSPF, O IA - OSPF inter area, O E1 - OSPF external type 1,
       O E2 - OSPF external type 2, O N1 - OSPF NSSA external type 1,
       O N2 - OSPF NSSA external type2, O3 - OSPFv3,
       O3 IA - OSPFv3 inter area, O3 E1 - OSPFv3 external type 1,
       O3 E2 - OSPFv3 external type 2,
       O3 N1 - OSPFv3 NSSA external type 1,
       O3 N2 - OSPFv3 NSSA external type2, B - Other BGP Routes,
       B I - iBGP, B E - eBGP, R - RIP, I L1 - IS-IS level 1,
       I L2 - IS-IS level 2, A B - BGP Aggregate,
       A O - OSPF Summary, NG - Nexthop Group Static Route,
       V - VXLAN Control Service, M - Martian,
       DH - DHCP client installed default route,
       DP - Dynamic Policy Route, L - VRF Leaked,
       G  - gRIBI, RC - Route Cache Route,
       CL - CBF Leaked Route

Gateway of last resort:
 S        0.0.0.0/0 [1/0]
           via 172.20.20.1, Management0

 B E      10.255.0.1/32 [20/0]
           via 10.255.255.12, Ethernet1
 B E      10.255.0.2/32 [20/0]
           via 10.255.255.14, Ethernet2
 B E      10.255.0.3/32 [20/0]
           via 10.255.255.12, Ethernet1
           via 10.255.255.14, Ethernet2
 B E      10.255.0.4/32 [20/0]
           via 10.255.255.12, Ethernet1
           via 10.255.255.14, Ethernet2
 B I      10.255.0.5/32 [200/0]
           via 10.255.1.100, Vlan4093
 C        10.255.0.6/32
           directly connected, Loopback0
 B E      10.255.0.7/32 [20/0]
           via 10.255.255.12, Ethernet1
           via 10.255.255.14, Ethernet2
 B E      10.255.0.8/32 [20/0]
           via 10.255.255.12, Ethernet1
           via 10.255.255.14, Ethernet2
 C        10.255.1.68/31
           directly connected, Vlan4094
 C        10.255.1.100/31
           directly connected, Vlan4093
 C        10.255.255.12/31
           directly connected, Ethernet1
 C        10.255.255.14/31
           directly connected, Ethernet2
 C        172.20.20.0/24
           directly connected, Management0
 B E      192.168.1.3/32 [20/0]
           via 10.255.255.12, Ethernet1
           via 10.255.255.14, Ethernet2
 C        192.168.1.5/32
           directly connected, Loopback1
 B E      192.168.1.7/32 [20/0]
           via 10.255.255.12, Ethernet1
           via 10.255.255.14, Ethernet2
 B E      192.168.1.8/32 [20/0]
           via 10.255.255.12, Ethernet1
           via 10.255.255.14, Ethernet2
```
## show lldp neighbors

```
Last table change time   : 0:00:25 ago
Number of table inserts  : 3053
Number of table deletes  : 3031
Number of table drops    : 0
Number of table age-outs : 3031

Port          Neighbor Device ID       Neighbor Port ID    TTL
---------- ------------------------ ---------------------- ---
Et1           Spine1                   Ethernet4           120
Et2           Spine2                   Ethernet4           120
Et3           Leaf3                    Ethernet3           120
Et4           Leaf3                    Ethernet4           120
Et5           Host-C                   Ethernet2           120
Et6           Host-D                   Ethernet2           120
Ma0           Spine2                   Management0         120
Ma0           Host-E                   Management0         120
Ma0           ceos3                    Management0         120
Ma0           Host-B                   Management0         120
Ma0           Leaf2                    Management0         120
Ma0           Leaf5                    Management0         120
Ma0           Host-B                   Management0         120
Ma0           Host-D                   Management0         120
Ma0           Host-C                   Management0         120
Ma0           s1-leaf4                 Management0         120
Ma0           s1-leaf4                 Management0         120
Ma0           Host-D                   Management0         120
Ma0           Leaf3                    Management0         120
Ma0           Spine2                   Management0         120
Ma0           s1-leaf1                 Management0         120
Ma0           leaf1                    Management0         120
```
## show running-config

```
! Command: show running-config
! device: Leaf4 (cEOSLab, EOS-4.34.1F-42424637.4341F (engineering build))
!
no aaa root
!
username admin privilege 15 role network-admin secret sha512 $6$D6X/0n0DCU8E8ut8$2ZVNvYRrdHZieTLaJ4BnNOQD.FlrdzHAx0dkQapUN0FZpjpewlCSGDiF7.m8.q48CAke72NDGo1vpm0eZEclE.
!
management api http-commands
   protocol http
   no shutdown
   !
   vrf default
      no shutdown
!
daemon TerminAttr
   exec /usr/bin/TerminAttr -smashexcludes=ale,flexCounter,hardware,kni,pulse,strata -cvaddr=10.243.248.48:9910 -cvauth=token,/tmp/token -cvvrf=default -taillogs
   no shutdown
!
vlan internal order ascending range 1006 1199
!
no service interface inactive port-id allocation disabled
!
transceiver qsfp default-mode 4x10G
!
service routing protocols model multi-agent
!
hostname Leaf4
!
spanning-tree mode mstp
no spanning-tree vlan-id 4093-4094
!
system l1
   unsupported speed action error
   unsupported error-correction action error
!
vlan 21
   name VRF_A_VLAN_21
!
vlan 22
   name VRF_A_VLAN_22
!
vlan 3009
   name MLAG_L3_VRF_VRF_A
   trunk group MLAG
!
vlan 4093
   name MLAG_L3
   trunk group MLAG
!
vlan 4094
   name MLAG
   trunk group MLAG
!
vrf instance VRF_A
!
interface Port-Channel3
   description MLAG_Leaf3_Port-Channel3
   switchport mode trunk
   switchport trunk group MLAG
!
interface Port-Channel5
   description MLAG_PortChannel
   switchport trunk allowed vlan 21
   switchport mode trunk
   mlag 5
   spanning-tree portfast edge
!
interface Port-Channel6
   description MLAG_PortChannel
   switchport trunk allowed vlan 22
   switchport mode trunk
   mlag 6
   spanning-tree portfast edge
!
interface Ethernet1
   description P2P_Spine1_Ethernet4
   mtu 1500
   no switchport
   ip address 10.255.255.13/31
!
interface Ethernet2
   description P2P_Spine2_Ethernet4
   mtu 1500
   no switchport
   ip address 10.255.255.15/31
!
interface Ethernet3
   description MLAG_Leaf3_Ethernet3
   channel-group 3 mode active
!
interface Ethernet4
   description MLAG_Leaf3_Ethernet4
   channel-group 3 mode active
!
interface Ethernet5
   description SERVER_Host-C_Ethernet2
   channel-group 5 mode active
!
interface Ethernet6
   description SERVER_Host-D_Ethernet2
   channel-group 6 mode active
!
interface Loopback0
   description ROUTER_ID
   ip address 10.255.0.6/32
!
interface Loopback1
   description VXLAN_TUNNEL_SOURCE
   ip address 192.168.1.5/32
!
interface Management0
   description OOB_MANAGEMENT
   ip address 172.20.20.68/24
!
interface Vlan21
   description VRF_A_VLAN_21
   vrf VRF_A
   ip address virtual 10.10.21.254/24
!
interface Vlan22
   description VRF_A_VLAN_22
   vrf VRF_A
   ip address virtual 10.10.22.254/24
!
interface Vlan3009
   description MLAG_L3_VRF_VRF_A
   mtu 1500
   vrf VRF_A
   ip address 10.255.1.101/31
!
interface Vlan4093
   description MLAG_L3
   mtu 1500
   ip address 10.255.1.101/31
!
interface Vlan4094
   description MLAG
   mtu 1500
   no autostate
   ip address 10.255.1.69/31
!
interface Vxlan1
   description Leaf4_VTEP
   vxlan source-interface Loopback1
   vxlan virtual-router encapsulation mac-address mlag-system-id
   vxlan udp-port 4789
   vxlan vlan 21 vni 10021
   vxlan vlan 22 vni 10022
   vxlan vrf VRF_A vni 10
!
ip virtual-router mac-address 00:1c:73:00:00:99
!
ip routing
ip routing vrf VRF_A
!
ip prefix-list PL-LOOPBACKS-EVPN-OVERLAY
   seq 10 permit 10.255.0.0/27 eq 32
   seq 20 permit 192.168.1.0/27 eq 32
!
ip prefix-list PL-MLAG-PEER-VRFS
   seq 10 permit 10.255.1.100/31
!
mlag configuration
   domain-id LEAFS_POD2
   local-interface Vlan4094
   peer-address 10.255.1.68
   peer-link Port-Channel3
   reload-delay mlag 300
   reload-delay non-mlag 330
!
ip route 0.0.0.0/0 172.20.20.1
!
route-map RM-CONN-2-BGP permit 10
   match ip address prefix-list PL-LOOPBACKS-EVPN-OVERLAY
!
route-map RM-CONN-2-BGP-VRFS deny 10
   match ip address prefix-list PL-MLAG-PEER-VRFS
!
route-map RM-CONN-2-BGP-VRFS permit 20
!
route-map RM-MLAG-PEER-IN permit 10
   description Make routes learned over MLAG Peer-link less preferred on spines to ensure optimal routing
   set origin incomplete
!
router bfd
   multihop interval 300 min-rx 300 multiplier 3
!
router bgp 65002
   router-id 10.255.0.6
   no bgp default ipv4-unicast
   distance bgp 20 200 200
   maximum-paths 4 ecmp 4
   neighbor EVPN-OVERLAY-PEERS peer group
   neighbor EVPN-OVERLAY-PEERS update-source Loopback0
   neighbor EVPN-OVERLAY-PEERS bfd
   neighbor EVPN-OVERLAY-PEERS ebgp-multihop 3
   neighbor EVPN-OVERLAY-PEERS send-community
   neighbor EVPN-OVERLAY-PEERS maximum-routes 0
   neighbor IPv4-UNDERLAY-PEERS peer group
   neighbor IPv4-UNDERLAY-PEERS send-community
   neighbor IPv4-UNDERLAY-PEERS maximum-routes 12000
   neighbor MLAG-IPv4-UNDERLAY-PEER peer group
   neighbor MLAG-IPv4-UNDERLAY-PEER remote-as 65002
   neighbor MLAG-IPv4-UNDERLAY-PEER next-hop-self
   neighbor MLAG-IPv4-UNDERLAY-PEER description Leaf3
   neighbor MLAG-IPv4-UNDERLAY-PEER route-map RM-MLAG-PEER-IN in
   neighbor MLAG-IPv4-UNDERLAY-PEER send-community
   neighbor MLAG-IPv4-UNDERLAY-PEER maximum-routes 12000
   neighbor 10.255.0.1 peer group EVPN-OVERLAY-PEERS
   neighbor 10.255.0.1 remote-as 65100
   neighbor 10.255.0.1 description Spine1_Loopback0
   neighbor 10.255.0.2 peer group EVPN-OVERLAY-PEERS
   neighbor 10.255.0.2 remote-as 65100
   neighbor 10.255.0.2 description Spine2_Loopback0
   neighbor 10.255.1.100 peer group MLAG-IPv4-UNDERLAY-PEER
   neighbor 10.255.1.100 description Leaf3_Vlan4093
   neighbor 10.255.255.12 peer group IPv4-UNDERLAY-PEERS
   neighbor 10.255.255.12 remote-as 65100
   neighbor 10.255.255.12 description Spine1_Ethernet4
   neighbor 10.255.255.14 peer group IPv4-UNDERLAY-PEERS
   neighbor 10.255.255.14 remote-as 65100
   neighbor 10.255.255.14 description Spine2_Ethernet4
   redistribute connected route-map RM-CONN-2-BGP
   !
   vlan 21
      rd 10.255.0.6:10021
      route-target both 10021:10021
      redistribute learned
   !
   vlan 22
      rd 10.255.0.6:10022
      route-target both 10022:10022
      redistribute learned
   !
   address-family evpn
      neighbor EVPN-OVERLAY-PEERS activate
   !
   address-family ipv4
      no neighbor EVPN-OVERLAY-PEERS activate
      neighbor IPv4-UNDERLAY-PEERS activate
      neighbor MLAG-IPv4-UNDERLAY-PEER activate
   !
   vrf VRF_A
      rd 10.255.0.6:10
      route-target import evpn 10:10
      route-target export evpn 10:10
      router-id 10.255.0.6
      neighbor 10.255.1.100 peer group MLAG-IPv4-UNDERLAY-PEER
      neighbor 10.255.1.100 description Leaf3_Vlan3009
      redistribute connected route-map RM-CONN-2-BGP-VRFS
!
router multicast
   ipv4
      software-forwarding kernel
   !
   ipv6
      software-forwarding kernel
!
end
```
## show version

```
Arista cEOSLab
Hardware version: 
Serial number: SERHATLEAF4
Hardware MAC address: 001c.eaae.6ea0
System MAC address: 001c.eaae.6ea0

Software image version: 4.34.1F-42424637.4341F (engineering build)
Architecture: x86_64
Internal build version: 4.34.1F-42424637.4341F
Internal build ID: 7ba787cb-1add-413d-ab3e-8913ddc04827
Image format version: 1.0
Image optimization: None

Kernel version: 5.14.0-570.18.1.el9_6.x86_64

Uptime: 1 day, 22 hours and 28 minutes
Total memory: 263079940 kB
Free memory: 112046468 kB
```
## show vxlan vni

```
VNI to VLAN Mapping for Vxlan1
VNI         VLAN       Source       Interface           802.1Q Tag
----------- ---------- ------------ ------------------- ----------
10021       21         static       Port-Channel5       21        
                                    Vxlan1              21        
10022       22         static       Port-Channel6       22        
                                    Vxlan1              22        

VNI to dynamic VLAN Mapping for Vxlan1
VNI       VLAN       VRF         Source       
--------- ---------- ----------- ------------ 
10        4097       VRF_A       evpn
```
