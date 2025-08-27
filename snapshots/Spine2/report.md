# Spine2 Commands Output

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
10.255.255.3      0:00:18  aac1.ab42.8789  Ethernet1
10.255.255.7      0:00:16  aac1.abe8.bdd8  Ethernet2
10.255.255.11     0:00:38  aac1.abe4.43c9  Ethernet3
10.255.255.15     0:00:03  aac1.abe2.fe46  Ethernet4
10.255.255.19     0:00:37  aac1.ab32.3ad7  Ethernet5
10.255.255.23     0:00:05  aac1.abe9.36d6  Ethernet6
172.20.20.1       0:00:00  9a5f.f8e6.7bd6  Management0
```
## show bgp evpn route-type imet

```
BGP routing table information for VRF default
Router identifier 10.255.0.2, local AS number 65100
Route status codes: * - valid, > - active, S - Stale, E - ECMP head, e - ECMP
                    c - Contributing to ECMP, % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
 * >      RD: 10.255.0.3:10011 imet 192.168.1.3
                                 192.168.1.3           -       100     0       65001 i
 * >      RD: 10.255.0.3:10012 imet 192.168.1.3
                                 192.168.1.3           -       100     0       65001 i
 * >      RD: 10.255.0.4:10011 imet 192.168.1.3
                                 192.168.1.3           -       100     0       65001 i
 * >      RD: 10.255.0.4:10012 imet 192.168.1.3
                                 192.168.1.3           -       100     0       65001 i
 * >      RD: 10.255.0.5:10021 imet 192.168.1.5
                                 192.168.1.5           -       100     0       65002 i
 * >      RD: 10.255.0.5:10022 imet 192.168.1.5
                                 192.168.1.5           -       100     0       65002 i
 * >      RD: 10.255.0.6:10021 imet 192.168.1.5
                                 192.168.1.5           -       100     0       65002 i
 * >      RD: 10.255.0.6:10022 imet 192.168.1.5
                                 192.168.1.5           -       100     0       65002 i
 * >      RD: 10.255.0.7:10031 imet 192.168.1.7
                                 192.168.1.7           -       100     0       65005 i
 * >      RD: 10.255.0.7:10032 imet 192.168.1.7
                                 192.168.1.7           -       100     0       65005 i
 * >      RD: 10.255.0.8:10031 imet 192.168.1.8
                                 192.168.1.8           -       100     0       65006 i
 * >      RD: 10.255.0.8:10032 imet 192.168.1.8
                                 192.168.1.8           -       100     0       65006 i
```
## show bgp evpn route-type ip-prefix

```
BGP routing table information for VRF default
Router identifier 10.255.0.2, local AS number 65100
Route status codes: * - valid, > - active, S - Stale, E - ECMP head, e - ECMP
                    c - Contributing to ECMP, % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
 * >      RD: 10.255.0.3:10 ip-prefix 10.10.11.0/24
                                 192.168.1.3           -       100     0       65001 i
 * >      RD: 10.255.0.4:10 ip-prefix 10.10.11.0/24
                                 192.168.1.3           -       100     0       65001 i
 * >      RD: 10.255.0.3:10 ip-prefix 10.10.12.0/24
                                 192.168.1.3           -       100     0       65001 i
 * >      RD: 10.255.0.4:10 ip-prefix 10.10.12.0/24
                                 192.168.1.3           -       100     0       65001 i
 * >      RD: 10.255.0.5:10 ip-prefix 10.10.21.0/24
                                 192.168.1.5           -       100     0       65002 i
 * >      RD: 10.255.0.6:10 ip-prefix 10.10.21.0/24
                                 192.168.1.5           -       100     0       65002 i
 * >      RD: 10.255.0.5:10 ip-prefix 10.10.22.0/24
                                 192.168.1.5           -       100     0       65002 i
 * >      RD: 10.255.0.6:10 ip-prefix 10.10.22.0/24
                                 192.168.1.5           -       100     0       65002 i
 * >      RD: 10.255.0.7:10 ip-prefix 10.10.31.0/24
                                 192.168.1.7           -       100     0       65005 i
 * >      RD: 10.255.0.8:10 ip-prefix 10.10.31.0/24
                                 192.168.1.8           -       100     0       65006 i
 * >      RD: 10.255.0.7:10 ip-prefix 10.10.32.0/24
                                 192.168.1.7           -       100     0       65005 i
 * >      RD: 10.255.0.8:10 ip-prefix 10.10.32.0/24
                                 192.168.1.8           -       100     0       65006 i
```
## show bgp evpn route-type mac-ip

```
BGP routing table information for VRF default
Router identifier 10.255.0.2, local AS number 65100
Route status codes: * - valid, > - active, S - Stale, E - ECMP head, e - ECMP
                    c - Contributing to ECMP, % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  LocPref Weight  Path
```
## show bgp evpn summary

```
BGP summary information for VRF default
Router identifier 10.255.0.2, local AS number 65100
Neighbor Status Codes: m - Under maintenance
  Description              Neighbor   V AS           MsgRcvd   MsgSent  InQ OutQ  Up/Down State   PfxRcd PfxAcc PfxAdv
  Leaf1_Loopback0          10.255.0.3 4 65001            116       114    0    0 01:17:27 Estab   4      4      20
  Leaf2_Loopback0          10.255.0.4 4 65001            115       114    0    0 01:17:26 Estab   4      4      20
  Leaf3_Loopback0          10.255.0.5 4 65002            115       110    0    0 01:17:26 Estab   4      4      20
  Leaf4_Loopback0          10.255.0.6 4 65002            111       108    0    0 01:17:23 Estab   4      4      20
  Leaf5_Loopback0          10.255.0.7 4 65005            107       107    0    0 01:17:22 Estab   4      4      20
  Leaf6_Loopback0          10.255.0.8 4 65006             97       108    0    0 01:17:22 Estab   4      4      20
```
## show bgp summary

```
BGP summary information for VRF default
Router identifier 10.255.0.2, local AS number 65100
Neighbor               AS Session State AFI/SAFI                AFI/SAFI State   NLRI Rcd   NLRI Acc   NLRI Adv
------------- ----------- ------------- ----------------------- -------------- ---------- ---------- ----------
10.255.0.3          65001 Established   L2VPN EVPN              Negotiated              4          4         20
10.255.0.4          65001 Established   L2VPN EVPN              Negotiated              4          4         20
10.255.0.5          65002 Established   L2VPN EVPN              Negotiated              4          4         20
10.255.0.6          65002 Established   L2VPN EVPN              Negotiated              4          4         20
10.255.0.7          65005 Established   L2VPN EVPN              Negotiated              4          4         20
10.255.0.8          65006 Established   L2VPN EVPN              Negotiated              4          4         20
10.255.255.3        65001 Established   IPv4 Unicast            Negotiated              3          3          9
10.255.255.7        65001 Established   IPv4 Unicast            Negotiated              3          3         10
10.255.255.11       65002 Established   IPv4 Unicast            Negotiated              3          3          9
10.255.255.15       65002 Established   IPv4 Unicast            Negotiated              3          3         10
10.255.255.19       65005 Established   IPv4 Unicast            Negotiated              2          2          9
10.255.255.23       65006 Established   IPv4 Unicast            Negotiated              2          2          9
```
## show interfaces description

```
Interface                      Status         Protocol           Description
Et1                            up             up                 P2P_Leaf1_Ethernet2
Et2                            up             up                 P2P_Leaf2_Ethernet2
Et3                            up             up                 P2P_Leaf3_Ethernet2
Et4                            up             up                 P2P_Leaf4_Ethernet2
Et5                            up             up                 P2P_Leaf5_Ethernet2
Et6                            up             up                 P2P_Leaf6_Ethernet2
Lo0                            up             up                 ROUTER_ID
Ma0                            up             up                 OOB_MANAGEMENT
```
## show interfaces vxlan1

```
not supported command
```
## show ip bgp

```
BGP routing table information for VRF default
Router identifier 10.255.0.2, local AS number 65100
Route status codes: s - suppressed contributor, * - valid, > - active, E - ECMP head, e - ECMP
                    S - Stale, c - Contributing to ECMP, b - backup, L - labeled-unicast, q - Pending FIB install
                    % - Pending best path selection
Origin codes: i - IGP, e - EGP, ? - incomplete
RPKI Origin Validation codes: V - valid, I - invalid, U - unknown
AS Path Attributes: Or-ID - Originator ID, C-LST - Cluster List, LL Nexthop - Link Local Nexthop

          Network                Next Hop              Metric  AIGP       LocPref Weight  Path
 * >      10.255.0.2/32          -                     -       -          -       0       i
 * >      10.255.0.3/32          10.255.255.3          0       -          100     0       65001 i
 *        10.255.0.3/32          10.255.255.7          0       -          100     0       65001 ?
 * >      10.255.0.4/32          10.255.255.7          0       -          100     0       65001 i
 *        10.255.0.4/32          10.255.255.3          0       -          100     0       65001 ?
 * >      10.255.0.5/32          10.255.255.11         0       -          100     0       65002 i
 *        10.255.0.5/32          10.255.255.15         0       -          100     0       65002 ?
 * >      10.255.0.6/32          10.255.255.15         0       -          100     0       65002 i
 *        10.255.0.6/32          10.255.255.11         0       -          100     0       65002 ?
 * >      10.255.0.7/32          10.255.255.19         0       -          100     0       65005 i
 * >      10.255.0.8/32          10.255.255.23         0       -          100     0       65006 i
 * >Ec    192.168.1.3/32         10.255.255.3          0       -          100     0       65001 i
 *  ec    192.168.1.3/32         10.255.255.7          0       -          100     0       65001 i
 * >Ec    192.168.1.5/32         10.255.255.11         0       -          100     0       65002 i
 *  ec    192.168.1.5/32         10.255.255.15         0       -          100     0       65002 i
 * >      192.168.1.7/32         10.255.255.19         0       -          100     0       65005 i
 * >      192.168.1.8/32         10.255.255.23         0       -          100     0       65006 i
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

 C        10.255.0.2/32
           directly connected, Loopback0
 B E      10.255.0.3/32 [20/0]
           via 10.255.255.3, Ethernet1
 B E      10.255.0.4/32 [20/0]
           via 10.255.255.7, Ethernet2
 B E      10.255.0.5/32 [20/0]
           via 10.255.255.11, Ethernet3
 B E      10.255.0.6/32 [20/0]
           via 10.255.255.15, Ethernet4
 B E      10.255.0.7/32 [20/0]
           via 10.255.255.19, Ethernet5
 B E      10.255.0.8/32 [20/0]
           via 10.255.255.23, Ethernet6
 C        10.255.255.2/31
           directly connected, Ethernet1
 C        10.255.255.6/31
           directly connected, Ethernet2
 C        10.255.255.10/31
           directly connected, Ethernet3
 C        10.255.255.14/31
           directly connected, Ethernet4
 C        10.255.255.18/31
           directly connected, Ethernet5
 C        10.255.255.22/31
           directly connected, Ethernet6
 C        172.20.20.0/24
           directly connected, Management0
 B E      192.168.1.3/32 [20/0]
           via 10.255.255.3, Ethernet1
           via 10.255.255.7, Ethernet2
 B E      192.168.1.5/32 [20/0]
           via 10.255.255.11, Ethernet3
           via 10.255.255.15, Ethernet4
 B E      192.168.1.7/32 [20/0]
           via 10.255.255.19, Ethernet5
 B E      192.168.1.8/32 [20/0]
           via 10.255.255.23, Ethernet6
```
## show lldp neighbors

```
Last table change time   : 0:07:41 ago
Number of table inserts  : 3138
Number of table deletes  : 3116
Number of table drops    : 0
Number of table age-outs : 3116

Port          Neighbor Device ID       Neighbor Port ID    TTL
---------- ------------------------ ---------------------- ---
Et1           Leaf1                    Ethernet2           120
Et2           Leaf2                    Ethernet2           120
Et3           Leaf3                    Ethernet2           120
Et4           Leaf4                    Ethernet2           120
Et5           Leaf5                    Ethernet2           120
Et6           Leaf6                    Ethernet2           120
Ma0           Host-F                   Management0         120
Ma0           Host-A                   Management0         120
Ma0           Host-A                   Management0         120
Ma0           Leaf2                    Management0         120
Ma0           Host-C                   Management0         120
Ma0           ceos2                    Management0         120
Ma0           Spine1                   Management0         120
Ma0           Leaf6                    Management0         120
Ma0           Leaf6                    Management0         120
Ma0           s1-host2                 Management0         120
Ma0           Host-D                   Management0         120
Ma0           sw1                      Management0         120
Ma0           Spine1                   Management0         120
Ma0           s1-spine2                Management0         120
Ma0           Host-E                   Management0         120
Ma0           Leaf1                    Management0         120
```
## show running-config

```
! Command: show running-config
! device: Spine2 (cEOSLab, EOS-4.34.1F-42424637.4341F (engineering build))
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
hostname Spine2
!
spanning-tree mode mstp
!
system l1
   unsupported speed action error
   unsupported error-correction action error
!
interface Ethernet1
   description P2P_Leaf1_Ethernet2
   mtu 1500
   no switchport
   ip address 10.255.255.2/31
!
interface Ethernet2
   description P2P_Leaf2_Ethernet2
   mtu 1500
   no switchport
   ip address 10.255.255.6/31
!
interface Ethernet3
   description P2P_Leaf3_Ethernet2
   mtu 1500
   no switchport
   ip address 10.255.255.10/31
!
interface Ethernet4
   description P2P_Leaf4_Ethernet2
   mtu 1500
   no switchport
   ip address 10.255.255.14/31
!
interface Ethernet5
   description P2P_Leaf5_Ethernet2
   mtu 1500
   no switchport
   ip address 10.255.255.18/31
!
interface Ethernet6
   description P2P_Leaf6_Ethernet2
   mtu 1500
   no switchport
   ip address 10.255.255.22/31
!
interface Loopback0
   description ROUTER_ID
   ip address 10.255.0.2/32
!
interface Management0
   description OOB_MANAGEMENT
   ip address 172.20.20.66/24
!
ip routing
!
ip prefix-list PL-LOOPBACKS-EVPN-OVERLAY
   seq 10 permit 10.255.0.0/27 eq 32
!
ip route 0.0.0.0/0 172.20.20.1
!
route-map RM-CONN-2-BGP permit 10
   match ip address prefix-list PL-LOOPBACKS-EVPN-OVERLAY
!
router bfd
   multihop interval 300 min-rx 300 multiplier 3
!
router bgp 65100
   router-id 10.255.0.2
   no bgp default ipv4-unicast
   distance bgp 20 200 200
   maximum-paths 4 ecmp 4
   neighbor EVPN-OVERLAY-PEERS peer group
   neighbor EVPN-OVERLAY-PEERS next-hop-unchanged
   neighbor EVPN-OVERLAY-PEERS update-source Loopback0
   neighbor EVPN-OVERLAY-PEERS bfd
   neighbor EVPN-OVERLAY-PEERS ebgp-multihop 3
   neighbor EVPN-OVERLAY-PEERS send-community
   neighbor EVPN-OVERLAY-PEERS maximum-routes 0
   neighbor IPv4-UNDERLAY-PEERS peer group
   neighbor IPv4-UNDERLAY-PEERS send-community
   neighbor IPv4-UNDERLAY-PEERS maximum-routes 12000
   neighbor 10.255.0.3 peer group EVPN-OVERLAY-PEERS
   neighbor 10.255.0.3 remote-as 65001
   neighbor 10.255.0.3 description Leaf1_Loopback0
   neighbor 10.255.0.4 peer group EVPN-OVERLAY-PEERS
   neighbor 10.255.0.4 remote-as 65001
   neighbor 10.255.0.4 description Leaf2_Loopback0
   neighbor 10.255.0.5 peer group EVPN-OVERLAY-PEERS
   neighbor 10.255.0.5 remote-as 65002
   neighbor 10.255.0.5 description Leaf3_Loopback0
   neighbor 10.255.0.6 peer group EVPN-OVERLAY-PEERS
   neighbor 10.255.0.6 remote-as 65002
   neighbor 10.255.0.6 description Leaf4_Loopback0
   neighbor 10.255.0.7 peer group EVPN-OVERLAY-PEERS
   neighbor 10.255.0.7 remote-as 65005
   neighbor 10.255.0.7 description Leaf5_Loopback0
   neighbor 10.255.0.8 peer group EVPN-OVERLAY-PEERS
   neighbor 10.255.0.8 remote-as 65006
   neighbor 10.255.0.8 description Leaf6_Loopback0
   neighbor 10.255.255.3 peer group IPv4-UNDERLAY-PEERS
   neighbor 10.255.255.3 remote-as 65001
   neighbor 10.255.255.3 description Leaf1_Ethernet2
   neighbor 10.255.255.7 peer group IPv4-UNDERLAY-PEERS
   neighbor 10.255.255.7 remote-as 65001
   neighbor 10.255.255.7 description Leaf2_Ethernet2
   neighbor 10.255.255.11 peer group IPv4-UNDERLAY-PEERS
   neighbor 10.255.255.11 remote-as 65002
   neighbor 10.255.255.11 description Leaf3_Ethernet2
   neighbor 10.255.255.15 peer group IPv4-UNDERLAY-PEERS
   neighbor 10.255.255.15 remote-as 65002
   neighbor 10.255.255.15 description Leaf4_Ethernet2
   neighbor 10.255.255.19 peer group IPv4-UNDERLAY-PEERS
   neighbor 10.255.255.19 remote-as 65005
   neighbor 10.255.255.19 description Leaf5_Ethernet2
   neighbor 10.255.255.23 peer group IPv4-UNDERLAY-PEERS
   neighbor 10.255.255.23 remote-as 65006
   neighbor 10.255.255.23 description Leaf6_Ethernet2
   redistribute connected route-map RM-CONN-2-BGP
   !
   address-family evpn
      neighbor EVPN-OVERLAY-PEERS activate
   !
   address-family ipv4
      no neighbor EVPN-OVERLAY-PEERS activate
      neighbor IPv4-UNDERLAY-PEERS activate
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
Serial number: SERHATSPINE2
Hardware MAC address: 001c.eaae.b896
System MAC address: 001c.eaae.b896

Software image version: 4.34.1F-42424637.4341F (engineering build)
Architecture: x86_64
Internal build version: 4.34.1F-42424637.4341F
Internal build ID: 7ba787cb-1add-413d-ab3e-8913ddc04827
Image format version: 1.0
Image optimization: None

Kernel version: 5.14.0-570.18.1.el9_6.x86_64

Uptime: 1 day, 22 hours and 28 minutes
Total memory: 263079940 kB
Free memory: 112349936 kB
```
## show vxlan vni

```

```
