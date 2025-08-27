# Leaf6 Commands Output

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
10.255.255.20     0:00:22  aac1.ab9b.123b  Ethernet1
10.255.255.22     0:00:07  aac1.ab94.4672  Ethernet2
172.20.20.1       0:00:00  9a5f.f8e6.7bd6  Management0
```
## show bgp evpn route-type imet

```
BGP routing table information for VRF default
Router identifier 10.255.0.8, local AS number 65006
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
 * >Ec    RD: 10.255.0.5:10021 imet 192.168.1.5
                                 192.168.1.5           -       100     0       65100 65002 i
 *  ec    RD: 10.255.0.5:10021 imet 192.168.1.5
                                 192.168.1.5           -       100     0       65100 65002 i
 * >Ec    RD: 10.255.0.5:10022 imet 192.168.1.5
                                 192.168.1.5           -       100     0       65100 65002 i
 *  ec    RD: 10.255.0.5:10022 imet 192.168.1.5
                                 192.168.1.5           -       100     0       65100 65002 i
 * >Ec    RD: 10.255.0.6:10021 imet 192.168.1.5
                                 192.168.1.5           -       100     0       65100 65002 i
 *  ec    RD: 10.255.0.6:10021 imet 192.168.1.5
                                 192.168.1.5           -       100     0       65100 65002 i
 * >Ec    RD: 10.255.0.6:10022 imet 192.168.1.5
                                 192.168.1.5           -       100     0       65100 65002 i
 *  ec    RD: 10.255.0.6:10022 imet 192.168.1.5
                                 192.168.1.5           -       100     0       65100 65002 i
 * >Ec    RD: 10.255.0.7:10031 imet 192.168.1.7
                                 192.168.1.7           -       100     0       65100 65005 i
 *  ec    RD: 10.255.0.7:10031 imet 192.168.1.7
                                 192.168.1.7           -       100     0       65100 65005 i
 * >Ec    RD: 10.255.0.7:10032 imet 192.168.1.7
                                 192.168.1.7           -       100     0       65100 65005 i
 *  ec    RD: 10.255.0.7:10032 imet 192.168.1.7
                                 192.168.1.7           -       100     0       65100 65005 i
 * >      RD: 10.255.0.8:10031 imet 192.168.1.8
                                 -                     -       -       0       i
 * >      RD: 10.255.0.8:10032 imet 192.168.1.8
                                 -                     -       -       0       i
```
## show bgp evpn route-type ip-prefix

```
BGP routing table information for VRF default
Router identifier 10.255.0.8, local AS number 65006
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
 * >Ec    RD: 10.255.0.3:10 ip-prefix 10.10.12.0/24
                                 192.168.1.3           -       100     0       65100 65001 i
 *  ec    RD: 10.255.0.3:10 ip-prefix 10.10.12.0/24
                                 192.168.1.3           -       100     0       65100 65001 i
 * >Ec    RD: 10.255.0.4:10 ip-prefix 10.10.12.0/24
                                 192.168.1.3           -       100     0       65100 65001 i
 *  ec    RD: 10.255.0.4:10 ip-prefix 10.10.12.0/24
                                 192.168.1.3           -       100     0       65100 65001 i
 * >Ec    RD: 10.255.0.5:10 ip-prefix 10.10.21.0/24
                                 192.168.1.5           -       100     0       65100 65002 i
 *  ec    RD: 10.255.0.5:10 ip-prefix 10.10.21.0/24
                                 192.168.1.5           -       100     0       65100 65002 i
 * >Ec    RD: 10.255.0.6:10 ip-prefix 10.10.21.0/24
                                 192.168.1.5           -       100     0       65100 65002 i
 *  ec    RD: 10.255.0.6:10 ip-prefix 10.10.21.0/24
                                 192.168.1.5           -       100     0       65100 65002 i
 * >Ec    RD: 10.255.0.5:10 ip-prefix 10.10.22.0/24
                                 192.168.1.5           -       100     0       65100 65002 i
 *  ec    RD: 10.255.0.5:10 ip-prefix 10.10.22.0/24
                                 192.168.1.5           -       100     0       65100 65002 i
 * >Ec    RD: 10.255.0.6:10 ip-prefix 10.10.22.0/24
                                 192.168.1.5           -       100     0       65100 65002 i
 *  ec    RD: 10.255.0.6:10 ip-prefix 10.10.22.0/24
                                 192.168.1.5           -       100     0       65100 65002 i
 * >Ec    RD: 10.255.0.7:10 ip-prefix 10.10.31.0/24
                                 192.168.1.7           -       100     0       65100 65005 i
 *  ec    RD: 10.255.0.7:10 ip-prefix 10.10.31.0/24
                                 192.168.1.7           -       100     0       65100 65005 i
 * >      RD: 10.255.0.8:10 ip-prefix 10.10.31.0/24
                                 -                     -       -       0       i
 * >Ec    RD: 10.255.0.7:10 ip-prefix 10.10.32.0/24
                                 192.168.1.7           -       100     0       65100 65005 i
 *  ec    RD: 10.255.0.7:10 ip-prefix 10.10.32.0/24
                                 192.168.1.7           -       100     0       65100 65005 i
 * >      RD: 10.255.0.8:10 ip-prefix 10.10.32.0/24
                                 -                     -       -       0       i
```
## show bgp evpn route-type mac-ip

```
BGP routing table information for VRF default
Router identifier 10.255.0.8, local AS number 65006
Route status codes: * - valid, > - active, S - Stale, E - ECMP head, e - ECMP
                    c - Contributing to ECMP, % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
```
## show bgp evpn summary

```
BGP summary information for VRF default
Router identifier 10.255.0.8, local AS number 65006
Neighbor Status Codes: m - Under maintenance
  Description              Neighbor   V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc PfxAdv
  Spine1_Loopback0         10.255.0.1 4 65100            103       107    0    0 01:17:30 Estab   20     20     24
  Spine2_Loopback0         10.255.0.2 4 65100            109        97    0    0 01:17:32 Estab   20     20     4
```
## show bgp summary

```
BGP summary information for VRF default
Router identifier 10.255.0.8, local AS number 65006
Neighbor               AS Session State AFI/SAFI                AFI/SAFI State   NLRI Rcd   NLRI Acc   NLRI Adv
------------- ----------- ------------- ----------------------- -------------- ---------- ---------- ----------
10.255.0.1          65100 Established   L2VPN EVPN              Negotiated             20         20         24
10.255.0.2          65100 Established   L2VPN EVPN              Negotiated             20         20          4
10.255.255.20       65100 Established   IPv4 Unicast            Negotiated              9          9          6
10.255.255.22       65100 Established   IPv4 Unicast            Negotiated              9          9          8
```
## show interfaces description

```
Interface                      Status         Protocol           Description
Et1                            up             up                 P2P_Spine1_Ethernet6
Et2                            up             up                 P2P_Spine2_Ethernet6
Et5                            up             up                 SERVER_Host-E_Ethernet2
Et6                            up             up                 SERVER_Host-F_Ethernet2
Lo0                            up             up                 ROUTER_ID
Lo1                            up             up                 VXLAN_TUNNEL_SOURCE
Ma0                            up             up                 OOB_MANAGEMENT
Po5                            down           lowerlayerdown     EVPN_AA_PortChannel
Po6                            down           lowerlayerdown     EVPN_AA_PortChannel
Vl31                           up             up                 VRF_A_VLAN_31
Vl32                           up             up                 VRF_A_VLAN_32
Vl4097                         up             up                 
Vx1                            up             up                 Leaf6_VTEP
```
## show interfaces vxlan1

```
Vxlan1 is up, line protocol is up (connected)
  Hardware is Vxlan
  Description: Leaf6_VTEP
  Source interface is Loopback1 and is active with 192.168.1.8
  Listening on UDP port 4789
  Replication/Flood Mode is headend with Flood List Source: EVPN
  Remote MAC learning via EVPN
  VNI mapping to VLANs
  Static VLAN to VNI mapping is 
    [31, 10031]       [32, 10032]      
  Dynamic VLAN to VNI mapping for 'evpn' is
    [4097, 10]       
  Note: All Dynamic VLANs used by VCS are internal VLANs.
        Use 'show vxlan vni' for details.
  Static VRF to VNI mapping is 
   [VRF_A, 10]
  Headend replication flood vtep list is:
    31 192.168.1.7    
    32 192.168.1.7    
  Shared Router MAC is 0000.0000.0000
```
## show ip bgp

```
BGP routing table information for VRF default
Router identifier 10.255.0.8, local AS number 65006
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast, q - Pending FIB install
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
RPKI Origin Validation codes: V - valid, I - invalid, U - unknown
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  AIGP       LocPref Weight  Path
 * >      10.255.0.1/32          10.255.255.20         0       -          100     0       65100 i
 * >      10.255.0.2/32          10.255.255.22         0       -          100     0       65100 i
 * >Ec    10.255.0.3/32          10.255.255.22         0       -          100     0       65100 65001 i
 *  ec    10.255.0.3/32          10.255.255.20         0       -          100     0       65100 65001 i
 * >Ec    10.255.0.4/32          10.255.255.20         0       -          100     0       65100 65001 i
 *  ec    10.255.0.4/32          10.255.255.22         0       -          100     0       65100 65001 i
 * >Ec    10.255.0.5/32          10.255.255.20         0       -          100     0       65100 65002 i
 *  ec    10.255.0.5/32          10.255.255.22         0       -          100     0       65100 65002 i
 * >Ec    10.255.0.6/32          10.255.255.20         0       -          100     0       65100 65002 i
 *  ec    10.255.0.6/32          10.255.255.22         0       -          100     0       65100 65002 i
 * >Ec    10.255.0.7/32          10.255.255.22         0       -          100     0       65100 65005 i
 *  ec    10.255.0.7/32          10.255.255.20         0       -          100     0       65100 65005 i
 * >      10.255.0.8/32          -                     -       -          -       0       i
 * >Ec    192.168.1.3/32         10.255.255.20         0       -          100     0       65100 65001 i
 *  ec    192.168.1.3/32         10.255.255.22         0       -          100     0       65100 65001 i
 * >Ec    192.168.1.5/32         10.255.255.20         0       -          100     0       65100 65002 i
 *  ec    192.168.1.5/32         10.255.255.22         0       -          100     0       65100 65002 i
 * >Ec    192.168.1.7/32         10.255.255.22         0       -          100     0       65100 65005 i
 *  ec    192.168.1.7/32         10.255.255.20         0       -          100     0       65100 65005 i
 * >      192.168.1.8/32         -                     -       -          -       0       i
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
           via 10.255.255.20, Ethernet1
 B E      10.255.0.2/32 [20/0]
           via 10.255.255.22, Ethernet2
 B E      10.255.0.3/32 [20/0]
           via 10.255.255.20, Ethernet1
           via 10.255.255.22, Ethernet2
 B E      10.255.0.4/32 [20/0]
           via 10.255.255.20, Ethernet1
           via 10.255.255.22, Ethernet2
 B E      10.255.0.5/32 [20/0]
           via 10.255.255.20, Ethernet1
           via 10.255.255.22, Ethernet2
 B E      10.255.0.6/32 [20/0]
           via 10.255.255.20, Ethernet1
           via 10.255.255.22, Ethernet2
 B E      10.255.0.7/32 [20/0]
           via 10.255.255.20, Ethernet1
           via 10.255.255.22, Ethernet2
 C        10.255.0.8/32
           directly connected, Loopback0
 C        10.255.255.20/31
           directly connected, Ethernet1
 C        10.255.255.22/31
           directly connected, Ethernet2
 C        172.20.20.0/24
           directly connected, Management0
 B E      192.168.1.3/32 [20/0]
           via 10.255.255.20, Ethernet1
           via 10.255.255.22, Ethernet2
 B E      192.168.1.5/32 [20/0]
           via 10.255.255.20, Ethernet1
           via 10.255.255.22, Ethernet2
 B E      192.168.1.7/32 [20/0]
           via 10.255.255.20, Ethernet1
           via 10.255.255.22, Ethernet2
 C        192.168.1.8/32
           directly connected, Loopback1
```
## show lldp neighbors

```
Last table change time   : 0:00:23 ago
Number of table inserts  : 3356
Number of table deletes  : 3336
Number of table drops    : 0
Number of table age-outs : 3336

Port          Neighbor Device ID       Neighbor Port ID    TTL
---------- ------------------------ ---------------------- ---
Et1           Spine1                   Ethernet6           120
Et2           Spine2                   Ethernet6           120
Et5           Host-E                   Ethernet2           120
Et6           Host-F                   Ethernet2           120
Ma0           ceos1                    Management0         120
Ma0           Spine2                   Management0         120
Ma0           Leaf6                    Management0         120
Ma0           Host-E                   Management0         120
Ma0           Host-F                   Management0         120
Ma0           sw4                      Management0         120
Ma0           Leaf5                    Management0         120
Ma0           s1-leaf4                 Management0         120
Ma0           Leaf1                    Management0         120
Ma0           Leaf3                    Management0         120
Ma0           Leaf2                    Management0         120
Ma0           Host-C                   Management0         120
Ma0           Host-E                   Management0         120
Ma0           Host-B                   Management0         120
Ma0           Leaf3                    Management0         120
Ma0           s1-spine1                Management0         120
```
## show running-config

```
! Command: show running-config
! device: Leaf6 (cEOSLab, EOS-4.34.1F-42424637.4341F (engineering build))
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
hostname Leaf6
!
spanning-tree mode mstp
!
system l1
   unsupported speed action error
   unsupported error-correction action error
!
vlan 31
   name VRF_A_VLAN_31
!
vlan 32
   name VRF_A_VLAN_32
!
vrf instance VRF_A
!
interface Port-Channel5
   description EVPN_AA_PortChannel
   switchport trunk allowed vlan 31
   switchport mode trunk
   !
   evpn ethernet-segment
      identifier 0000:0000:0000:0000:0001
      route-target import 00:00:00:00:00:01
   lacp system-id 0000.0000.0001
   spanning-tree portfast edge
!
interface Port-Channel6
   description EVPN_AA_PortChannel
   switchport trunk allowed vlan 32
   switchport mode trunk
   !
   evpn ethernet-segment
      identifier 0000:0000:0000:0000:0002
      route-target import 00:00:00:00:00:02
   lacp system-id 0000.0000.0002
   spanning-tree portfast edge
!
interface Ethernet1
   description P2P_Spine1_Ethernet6
   mtu 1500
   no switchport
   ip address 10.255.255.21/31
!
interface Ethernet2
   description P2P_Spine2_Ethernet6
   mtu 1500
   no switchport
   ip address 10.255.255.23/31
!
interface Ethernet5
   description SERVER_Host-E_Ethernet2
   channel-group 5 mode active
!
interface Ethernet6
   description SERVER_Host-F_Ethernet2
   channel-group 6 mode active
!
interface Loopback0
   description ROUTER_ID
   ip address 10.255.0.8/32
!
interface Loopback1
   description VXLAN_TUNNEL_SOURCE
   ip address 192.168.1.8/32
!
interface Management0
   description OOB_MANAGEMENT
   ip address 172.20.20.63/24
!
interface Vlan31
   description VRF_A_VLAN_31
   vrf VRF_A
   ip address virtual 10.10.31.254/24
!
interface Vlan32
   description VRF_A_VLAN_32
   vrf VRF_A
   ip address virtual 10.10.32.254/24
!
interface Vxlan1
   description Leaf6_VTEP
   vxlan source-interface Loopback1
   vxlan udp-port 4789
   vxlan vlan 31 vni 10031
   vxlan vlan 32 vni 10032
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
ip route 0.0.0.0/0 172.20.20.1
!
route-map RM-CONN-2-BGP permit 10
   match ip address prefix-list PL-LOOPBACKS-EVPN-OVERLAY
!
router bfd
   multihop interval 300 min-rx 300 multiplier 3
!
router bgp 65006
   router-id 10.255.0.8
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
   neighbor 10.255.0.1 peer group EVPN-OVERLAY-PEERS
   neighbor 10.255.0.1 remote-as 65100
   neighbor 10.255.0.1 description Spine1_Loopback0
   neighbor 10.255.0.2 peer group EVPN-OVERLAY-PEERS
   neighbor 10.255.0.2 remote-as 65100
   neighbor 10.255.0.2 description Spine2_Loopback0
   neighbor 10.255.255.20 peer group IPv4-UNDERLAY-PEERS
   neighbor 10.255.255.20 remote-as 65100
   neighbor 10.255.255.20 description Spine1_Ethernet6
   neighbor 10.255.255.22 peer group IPv4-UNDERLAY-PEERS
   neighbor 10.255.255.22 remote-as 65100
   neighbor 10.255.255.22 description Spine2_Ethernet6
   redistribute connected route-map RM-CONN-2-BGP
   !
   vlan 31
      rd 10.255.0.8:10031
      route-target both 10031:10031
      redistribute learned
   !
   vlan 32
      rd 10.255.0.8:10032
      route-target both 10032:10032
      redistribute learned
   !
   address-family evpn
      neighbor EVPN-OVERLAY-PEERS activate
   !
   address-family ipv4
      no neighbor EVPN-OVERLAY-PEERS activate
      neighbor IPv4-UNDERLAY-PEERS activate
   !
   vrf VRF_A
      rd 10.255.0.8:10
      route-target import evpn 10:10
      route-target export evpn 10:10
      router-id 10.255.0.8
      redistribute connected
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
Serial number: SERHATLEAF6
Hardware MAC address: 001c.eaae.1f73
System MAC address: 001c.eaae.1f73

Software image version: 4.34.1F-42424637.4341F (engineering build)
Architecture: x86_64
Internal build version: 4.34.1F-42424637.4341F
Internal build ID: 7ba787cb-1add-413d-ab3e-8913ddc04827
Image format version: 1.0
Image optimization: None

Kernel version: 5.14.0-570.18.1.el9_6.x86_64

Uptime: 1 day, 22 hours and 28 minutes
Total memory: 263079940 kB
Free memory: 112044452 kB
```
## show vxlan vni

```
VNI to VLAN Mapping for Vxlan1
VNI         VLAN       Source       Interface           802.1Q Tag
----------- ---------- ------------ ------------------- ----------
10031       31         static       Port-Channel5       31        
                                    Vxlan1              31        
10032       32         static       Port-Channel6       32        
                                    Vxlan1              32        

VNI to dynamic VLAN Mapping for Vxlan1
VNI       VLAN       VRF         Source       
--------- ---------- ----------- ------------ 
10        4097       VRF_A       evpn
```
