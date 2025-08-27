# Validate State Report

**Table of Contents:**

- [Validate State Report](validate-state-report)
  - [Test Results Summary](#test-results-summary)
  - [Failed Test Results Summary](#failed-test-results-summary)
  - [All Test Results](#all-test-results)

## Test Results Summary

### Summary Totals

| Total Tests | Total Tests Passed | Total Tests Failed | Total Tests Skipped |
| ----------- | ------------------ | ------------------ | ------------------- |
| 404 | 352 | 20 | 32 |

### Summary Totals Device Under Test

| Device Under Test | Total Tests | Tests Passed | Tests Failed | Tests Skipped | Categories Failed | Categories Skipped |
| ------------------| ----------- | ------------ | ------------ | ------------- | ----------------- | ------------------ |
| Leaf1 | 58 | 51 | 3 | 4 | Interfaces, System | Hardware |
| Leaf2 | 58 | 51 | 3 | 4 | Interfaces, System | Hardware |
| Leaf3 | 58 | 51 | 3 | 4 | Interfaces, System | Hardware |
| Leaf4 | 58 | 51 | 3 | 4 | Interfaces, System | Hardware |
| Leaf5 | 48 | 41 | 3 | 4 | Interfaces, System | Hardware |
| Leaf6 | 48 | 41 | 3 | 4 | Interfaces, System | Hardware |
| Spine1 | 38 | 33 | 1 | 4 | System | Hardware |
| Spine2 | 38 | 33 | 1 | 4 | System | Hardware |

### Summary Totals Per Category

| Test Category | Total Tests | Tests Passed | Tests Failed | Tests Skipped |
| ------------- | ----------- | ------------ | ------------ | ------------- |
| BGP | 52 | 52 | 0 | 0 |
| Connectivity | 116 | 116 | 0 | 0 |
| Hardware | 32 | 0 | 0 | 32 |
| Interfaces | 104 | 92 | 12 | 0 |
| MLAG | 4 | 4 | 0 | 0 |
| Routing | 80 | 80 | 0 | 0 |
| System | 16 | 8 | 8 | 0 |

## Failed Test Results Summary

| ID | Device Under Test | Categories | Test | Description | Inputs | Result | Messages |
| -- | ----------------- | ---------- | ---- | ----------- | ------ | -------| -------- |
| 35 | Leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel5 - MLAG_PortChannel = 'up' | FAIL | Port-Channel5 - Status mismatch - Expected: up/up, Actual: down/lowerLayerDown |
| 36 | Leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel6 - MLAG_PortChannel = 'up' | FAIL | Port-Channel6 - Status mismatch - Expected: up/up, Actual: down/lowerLayerDown |
| 57 | Leaf1 | System | VerifyNTP | Verifies if NTP is synchronised. | - | FAIL | NTP status mismatch - Expected: synchronised Actual: NTP is disabled. |
| 93 | Leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel5 - MLAG_PortChannel = 'up' | FAIL | Port-Channel5 - Status mismatch - Expected: up/up, Actual: down/lowerLayerDown |
| 94 | Leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel6 - MLAG_PortChannel = 'up' | FAIL | Port-Channel6 - Status mismatch - Expected: up/up, Actual: down/lowerLayerDown |
| 115 | Leaf2 | System | VerifyNTP | Verifies if NTP is synchronised. | - | FAIL | NTP status mismatch - Expected: synchronised Actual: NTP is disabled. |
| 151 | Leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel5 - MLAG_PortChannel = 'up' | FAIL | Port-Channel5 - Status mismatch - Expected: up/up, Actual: down/lowerLayerDown |
| 152 | Leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel6 - MLAG_PortChannel = 'up' | FAIL | Port-Channel6 - Status mismatch - Expected: up/up, Actual: down/lowerLayerDown |
| 173 | Leaf3 | System | VerifyNTP | Verifies if NTP is synchronised. | - | FAIL | NTP status mismatch - Expected: synchronised Actual: NTP is disabled. |
| 209 | Leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel5 - MLAG_PortChannel = 'up' | FAIL | Port-Channel5 - Status mismatch - Expected: up/up, Actual: down/lowerLayerDown |
| 210 | Leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel6 - MLAG_PortChannel = 'up' | FAIL | Port-Channel6 - Status mismatch - Expected: up/up, Actual: down/lowerLayerDown |
| 231 | Leaf4 | System | VerifyNTP | Verifies if NTP is synchronised. | - | FAIL | NTP status mismatch - Expected: synchronised Actual: NTP is disabled. |
| 261 | Leaf5 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel5 - EVPN_AA_PortChannel = 'up' | FAIL | Port-Channel5 - Status mismatch - Expected: up/up, Actual: down/lowerLayerDown |
| 262 | Leaf5 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel6 - EVPN_AA_PortChannel = 'up' | FAIL | Port-Channel6 - Status mismatch - Expected: up/up, Actual: down/lowerLayerDown |
| 279 | Leaf5 | System | VerifyNTP | Verifies if NTP is synchronised. | - | FAIL | NTP status mismatch - Expected: synchronised Actual: NTP is disabled. |
| 309 | Leaf6 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel5 - EVPN_AA_PortChannel = 'up' | FAIL | Port-Channel5 - Status mismatch - Expected: up/up, Actual: down/lowerLayerDown |
| 310 | Leaf6 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel6 - EVPN_AA_PortChannel = 'up' | FAIL | Port-Channel6 - Status mismatch - Expected: up/up, Actual: down/lowerLayerDown |
| 327 | Leaf6 | System | VerifyNTP | Verifies if NTP is synchronised. | - | FAIL | NTP status mismatch - Expected: synchronised Actual: NTP is disabled. |
| 365 | Spine1 | System | VerifyNTP | Verifies if NTP is synchronised. | - | FAIL | NTP status mismatch - Expected: synchronised Actual: NTP is disabled. |
| 403 | Spine2 | System | VerifyNTP | Verifies if NTP is synchronised. | - | FAIL | NTP status mismatch - Expected: synchronised Actual: NTP is disabled. |

## All Test Results

| ID | Device Under Test | Categories | Test | Description | Inputs | Result | Messages |
| -- | ----------------- | ---------- | ---- | ----------- | ------ | -------| -------- |
| 1 | Leaf1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: Spine1 (IP: 10.255.0.1) | PASS | - |
| 2 | Leaf1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: Spine2 (IP: 10.255.0.2) | PASS | - |
| 3 | Leaf1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: Leaf2 (IP: 10.255.1.97) | PASS | - |
| 4 | Leaf1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: Spine1 (IP: 10.255.255.0) | PASS | - |
| 5 | Leaf1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: Spine2 (IP: 10.255.255.2) | PASS | - |
| 6 | Leaf1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet1 - Remote: Spine1 Ethernet1 | PASS | - |
| 7 | Leaf1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet2 - Remote: Spine2 Ethernet1 | PASS | - |
| 8 | Leaf1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet3 - Remote: Leaf2 Ethernet3 | PASS | - |
| 9 | Leaf1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet4 - Remote: Leaf2 Ethernet4 | PASS | - |
| 10 | Leaf1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet5 - Remote: Host-A Ethernet1 | PASS | - |
| 11 | Leaf1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet6 - Remote: Host-B Ethernet1 | PASS | - |
| 12 | Leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.3) - Destination: Leaf1 Loopback0 (IP: 10.255.0.3) | PASS | - |
| 13 | Leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.3) - Destination: Leaf2 Loopback0 (IP: 10.255.0.4) | PASS | - |
| 14 | Leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.3) - Destination: Leaf3 Loopback0 (IP: 10.255.0.5) | PASS | - |
| 15 | Leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.3) - Destination: Leaf4 Loopback0 (IP: 10.255.0.6) | PASS | - |
| 16 | Leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.3) - Destination: Leaf5 Loopback0 (IP: 10.255.0.7) | PASS | - |
| 17 | Leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.3) - Destination: Leaf6 Loopback0 (IP: 10.255.0.8) | PASS | - |
| 18 | Leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.3) - Destination: Spine1 Loopback0 (IP: 10.255.0.1) | PASS | - |
| 19 | Leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.3) - Destination: Spine2 Loopback0 (IP: 10.255.0.2) | PASS | - |
| 20 | Leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet1 (IP: 10.255.255.1) - Destination: Spine1 Ethernet1 (IP: 10.255.255.0) | PASS | - |
| 21 | Leaf1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet2 (IP: 10.255.255.3) - Destination: Spine2 Ethernet1 (IP: 10.255.255.2) | PASS | - |
| 22 | Leaf1 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab |
| 23 | Leaf1 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab |
| 24 | Leaf1 | Hardware | VerifyTemperature | Verifies if the device temperature is within acceptable limits. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab |
| 25 | Leaf1 | Hardware | VerifyTransceiversManufacturers | Verifies if all the transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab |
| 26 | Leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet1 - P2P_Spine1_Ethernet1 = 'up' | PASS | - |
| 27 | Leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet2 - P2P_Spine2_Ethernet1 = 'up' | PASS | - |
| 28 | Leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet3 - MLAG_Leaf2_Ethernet3 = 'up' | PASS | - |
| 29 | Leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet4 - MLAG_Leaf2_Ethernet4 = 'up' | PASS | - |
| 30 | Leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet5 - SERVER_Host-A_Ethernet1 = 'up' | PASS | - |
| 31 | Leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet6 - SERVER_Host-B_Ethernet1 = 'up' | PASS | - |
| 32 | Leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback0 - ROUTER_ID = 'up' | PASS | - |
| 33 | Leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback1 - VXLAN_TUNNEL_SOURCE = 'up' | PASS | - |
| 34 | Leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel3 - MLAG_Leaf2_Port-Channel3 = 'up' | PASS | - |
| 35 | Leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel5 - MLAG_PortChannel = 'up' | FAIL | Port-Channel5 - Status mismatch - Expected: up/up, Actual: down/lowerLayerDown |
| 36 | Leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel6 - MLAG_PortChannel = 'up' | FAIL | Port-Channel6 - Status mismatch - Expected: up/up, Actual: down/lowerLayerDown |
| 37 | Leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan11 - VRF_A_VLAN_11 = 'up' | PASS | - |
| 38 | Leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan12 - VRF_A_VLAN_12 = 'up' | PASS | - |
| 39 | Leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan3009 - MLAG_L3_VRF_VRF_A = 'up' | PASS | - |
| 40 | Leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4093 - MLAG_L3 = 'up' | PASS | - |
| 41 | Leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4094 - MLAG = 'up' | PASS | - |
| 42 | Leaf1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vxlan1 = 'up' | PASS | - |
| 43 | Leaf1 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 44 | Leaf1 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | Routing protocol model: multi-agent | PASS | - |
| 45 | Leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.1 - Peer: Spine1 | PASS | - |
| 46 | Leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.2 - Peer: Spine2 | PASS | - |
| 47 | Leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.3 - Peer: Leaf1 | PASS | - |
| 48 | Leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.4 - Peer: Leaf2 | PASS | - |
| 49 | Leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.5 - Peer: Leaf3 | PASS | - |
| 50 | Leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.6 - Peer: Leaf4 | PASS | - |
| 51 | Leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.7 - Peer: Leaf5 | PASS | - |
| 52 | Leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.8 - Peer: Leaf6 | PASS | - |
| 53 | Leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 192.168.1.3 - Peer: Leaf1 | PASS | - |
| 54 | Leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 192.168.1.5 - Peer: Leaf3 | PASS | - |
| 55 | Leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 192.168.1.7 - Peer: Leaf5 | PASS | - |
| 56 | Leaf1 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 192.168.1.8 - Peer: Leaf6 | PASS | - |
| 57 | Leaf1 | System | VerifyNTP | Verifies if NTP is synchronised. | - | FAIL | NTP status mismatch - Expected: synchronised Actual: NTP is disabled. |
| 58 | Leaf1 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | PASS | - |
| 59 | Leaf2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: Spine1 (IP: 10.255.0.1) | PASS | - |
| 60 | Leaf2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: Spine2 (IP: 10.255.0.2) | PASS | - |
| 61 | Leaf2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: Leaf1 (IP: 10.255.1.96) | PASS | - |
| 62 | Leaf2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: Spine1 (IP: 10.255.255.4) | PASS | - |
| 63 | Leaf2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: Spine2 (IP: 10.255.255.6) | PASS | - |
| 64 | Leaf2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet1 - Remote: Spine1 Ethernet2 | PASS | - |
| 65 | Leaf2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet2 - Remote: Spine2 Ethernet2 | PASS | - |
| 66 | Leaf2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet3 - Remote: Leaf1 Ethernet3 | PASS | - |
| 67 | Leaf2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet4 - Remote: Leaf1 Ethernet4 | PASS | - |
| 68 | Leaf2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet5 - Remote: Host-A Ethernet2 | PASS | - |
| 69 | Leaf2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet6 - Remote: Host-B Ethernet2 | PASS | - |
| 70 | Leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.4) - Destination: Leaf1 Loopback0 (IP: 10.255.0.3) | PASS | - |
| 71 | Leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.4) - Destination: Leaf2 Loopback0 (IP: 10.255.0.4) | PASS | - |
| 72 | Leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.4) - Destination: Leaf3 Loopback0 (IP: 10.255.0.5) | PASS | - |
| 73 | Leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.4) - Destination: Leaf4 Loopback0 (IP: 10.255.0.6) | PASS | - |
| 74 | Leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.4) - Destination: Leaf5 Loopback0 (IP: 10.255.0.7) | PASS | - |
| 75 | Leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.4) - Destination: Leaf6 Loopback0 (IP: 10.255.0.8) | PASS | - |
| 76 | Leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.4) - Destination: Spine1 Loopback0 (IP: 10.255.0.1) | PASS | - |
| 77 | Leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.4) - Destination: Spine2 Loopback0 (IP: 10.255.0.2) | PASS | - |
| 78 | Leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet1 (IP: 10.255.255.5) - Destination: Spine1 Ethernet2 (IP: 10.255.255.4) | PASS | - |
| 79 | Leaf2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet2 (IP: 10.255.255.7) - Destination: Spine2 Ethernet2 (IP: 10.255.255.6) | PASS | - |
| 80 | Leaf2 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab |
| 81 | Leaf2 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab |
| 82 | Leaf2 | Hardware | VerifyTemperature | Verifies if the device temperature is within acceptable limits. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab |
| 83 | Leaf2 | Hardware | VerifyTransceiversManufacturers | Verifies if all the transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab |
| 84 | Leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet1 - P2P_Spine1_Ethernet2 = 'up' | PASS | - |
| 85 | Leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet2 - P2P_Spine2_Ethernet2 = 'up' | PASS | - |
| 86 | Leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet3 - MLAG_Leaf1_Ethernet3 = 'up' | PASS | - |
| 87 | Leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet4 - MLAG_Leaf1_Ethernet4 = 'up' | PASS | - |
| 88 | Leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet5 - SERVER_Host-A_Ethernet2 = 'up' | PASS | - |
| 89 | Leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet6 - SERVER_Host-B_Ethernet2 = 'up' | PASS | - |
| 90 | Leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback0 - ROUTER_ID = 'up' | PASS | - |
| 91 | Leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback1 - VXLAN_TUNNEL_SOURCE = 'up' | PASS | - |
| 92 | Leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel3 - MLAG_Leaf1_Port-Channel3 = 'up' | PASS | - |
| 93 | Leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel5 - MLAG_PortChannel = 'up' | FAIL | Port-Channel5 - Status mismatch - Expected: up/up, Actual: down/lowerLayerDown |
| 94 | Leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel6 - MLAG_PortChannel = 'up' | FAIL | Port-Channel6 - Status mismatch - Expected: up/up, Actual: down/lowerLayerDown |
| 95 | Leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan11 - VRF_A_VLAN_11 = 'up' | PASS | - |
| 96 | Leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan12 - VRF_A_VLAN_12 = 'up' | PASS | - |
| 97 | Leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan3009 - MLAG_L3_VRF_VRF_A = 'up' | PASS | - |
| 98 | Leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4093 - MLAG_L3 = 'up' | PASS | - |
| 99 | Leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4094 - MLAG = 'up' | PASS | - |
| 100 | Leaf2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vxlan1 = 'up' | PASS | - |
| 101 | Leaf2 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 102 | Leaf2 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | Routing protocol model: multi-agent | PASS | - |
| 103 | Leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.1 - Peer: Spine1 | PASS | - |
| 104 | Leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.2 - Peer: Spine2 | PASS | - |
| 105 | Leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.3 - Peer: Leaf1 | PASS | - |
| 106 | Leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.4 - Peer: Leaf2 | PASS | - |
| 107 | Leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.5 - Peer: Leaf3 | PASS | - |
| 108 | Leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.6 - Peer: Leaf4 | PASS | - |
| 109 | Leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.7 - Peer: Leaf5 | PASS | - |
| 110 | Leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.8 - Peer: Leaf6 | PASS | - |
| 111 | Leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 192.168.1.3 - Peer: Leaf1 | PASS | - |
| 112 | Leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 192.168.1.5 - Peer: Leaf3 | PASS | - |
| 113 | Leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 192.168.1.7 - Peer: Leaf5 | PASS | - |
| 114 | Leaf2 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 192.168.1.8 - Peer: Leaf6 | PASS | - |
| 115 | Leaf2 | System | VerifyNTP | Verifies if NTP is synchronised. | - | FAIL | NTP status mismatch - Expected: synchronised Actual: NTP is disabled. |
| 116 | Leaf2 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | PASS | - |
| 117 | Leaf3 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: Spine1 (IP: 10.255.0.1) | PASS | - |
| 118 | Leaf3 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: Spine2 (IP: 10.255.0.2) | PASS | - |
| 119 | Leaf3 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: Leaf4 (IP: 10.255.1.101) | PASS | - |
| 120 | Leaf3 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: Spine1 (IP: 10.255.255.8) | PASS | - |
| 121 | Leaf3 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: Spine2 (IP: 10.255.255.10) | PASS | - |
| 122 | Leaf3 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet1 - Remote: Spine1 Ethernet3 | PASS | - |
| 123 | Leaf3 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet2 - Remote: Spine2 Ethernet3 | PASS | - |
| 124 | Leaf3 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet3 - Remote: Leaf4 Ethernet3 | PASS | - |
| 125 | Leaf3 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet4 - Remote: Leaf4 Ethernet4 | PASS | - |
| 126 | Leaf3 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet5 - Remote: Host-C Ethernet1 | PASS | - |
| 127 | Leaf3 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet6 - Remote: Host-D Ethernet1 | PASS | - |
| 128 | Leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.5) - Destination: Leaf1 Loopback0 (IP: 10.255.0.3) | PASS | - |
| 129 | Leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.5) - Destination: Leaf2 Loopback0 (IP: 10.255.0.4) | PASS | - |
| 130 | Leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.5) - Destination: Leaf3 Loopback0 (IP: 10.255.0.5) | PASS | - |
| 131 | Leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.5) - Destination: Leaf4 Loopback0 (IP: 10.255.0.6) | PASS | - |
| 132 | Leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.5) - Destination: Leaf5 Loopback0 (IP: 10.255.0.7) | PASS | - |
| 133 | Leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.5) - Destination: Leaf6 Loopback0 (IP: 10.255.0.8) | PASS | - |
| 134 | Leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.5) - Destination: Spine1 Loopback0 (IP: 10.255.0.1) | PASS | - |
| 135 | Leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.5) - Destination: Spine2 Loopback0 (IP: 10.255.0.2) | PASS | - |
| 136 | Leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet1 (IP: 10.255.255.9) - Destination: Spine1 Ethernet3 (IP: 10.255.255.8) | PASS | - |
| 137 | Leaf3 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet2 (IP: 10.255.255.11) - Destination: Spine2 Ethernet3 (IP: 10.255.255.10) | PASS | - |
| 138 | Leaf3 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab |
| 139 | Leaf3 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab |
| 140 | Leaf3 | Hardware | VerifyTemperature | Verifies if the device temperature is within acceptable limits. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab |
| 141 | Leaf3 | Hardware | VerifyTransceiversManufacturers | Verifies if all the transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab |
| 142 | Leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet1 - P2P_Spine1_Ethernet3 = 'up' | PASS | - |
| 143 | Leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet2 - P2P_Spine2_Ethernet3 = 'up' | PASS | - |
| 144 | Leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet3 - MLAG_Leaf4_Ethernet3 = 'up' | PASS | - |
| 145 | Leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet4 - MLAG_Leaf4_Ethernet4 = 'up' | PASS | - |
| 146 | Leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet5 - SERVER_Host-C_Ethernet1 = 'up' | PASS | - |
| 147 | Leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet6 - SERVER_Host-D_Ethernet1 = 'up' | PASS | - |
| 148 | Leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback0 - ROUTER_ID = 'up' | PASS | - |
| 149 | Leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback1 - VXLAN_TUNNEL_SOURCE = 'up' | PASS | - |
| 150 | Leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel3 - MLAG_Leaf4_Port-Channel3 = 'up' | PASS | - |
| 151 | Leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel5 - MLAG_PortChannel = 'up' | FAIL | Port-Channel5 - Status mismatch - Expected: up/up, Actual: down/lowerLayerDown |
| 152 | Leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel6 - MLAG_PortChannel = 'up' | FAIL | Port-Channel6 - Status mismatch - Expected: up/up, Actual: down/lowerLayerDown |
| 153 | Leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan21 - VRF_A_VLAN_21 = 'up' | PASS | - |
| 154 | Leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan22 - VRF_A_VLAN_22 = 'up' | PASS | - |
| 155 | Leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan3009 - MLAG_L3_VRF_VRF_A = 'up' | PASS | - |
| 156 | Leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4093 - MLAG_L3 = 'up' | PASS | - |
| 157 | Leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4094 - MLAG = 'up' | PASS | - |
| 158 | Leaf3 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vxlan1 = 'up' | PASS | - |
| 159 | Leaf3 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 160 | Leaf3 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | Routing protocol model: multi-agent | PASS | - |
| 161 | Leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.1 - Peer: Spine1 | PASS | - |
| 162 | Leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.2 - Peer: Spine2 | PASS | - |
| 163 | Leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.3 - Peer: Leaf1 | PASS | - |
| 164 | Leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.4 - Peer: Leaf2 | PASS | - |
| 165 | Leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.5 - Peer: Leaf3 | PASS | - |
| 166 | Leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.6 - Peer: Leaf4 | PASS | - |
| 167 | Leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.7 - Peer: Leaf5 | PASS | - |
| 168 | Leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.8 - Peer: Leaf6 | PASS | - |
| 169 | Leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 192.168.1.3 - Peer: Leaf1 | PASS | - |
| 170 | Leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 192.168.1.5 - Peer: Leaf3 | PASS | - |
| 171 | Leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 192.168.1.7 - Peer: Leaf5 | PASS | - |
| 172 | Leaf3 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 192.168.1.8 - Peer: Leaf6 | PASS | - |
| 173 | Leaf3 | System | VerifyNTP | Verifies if NTP is synchronised. | - | FAIL | NTP status mismatch - Expected: synchronised Actual: NTP is disabled. |
| 174 | Leaf3 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | PASS | - |
| 175 | Leaf4 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: Spine1 (IP: 10.255.0.1) | PASS | - |
| 176 | Leaf4 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: Spine2 (IP: 10.255.0.2) | PASS | - |
| 177 | Leaf4 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: Leaf3 (IP: 10.255.1.100) | PASS | - |
| 178 | Leaf4 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: Spine1 (IP: 10.255.255.12) | PASS | - |
| 179 | Leaf4 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: Spine2 (IP: 10.255.255.14) | PASS | - |
| 180 | Leaf4 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet1 - Remote: Spine1 Ethernet4 | PASS | - |
| 181 | Leaf4 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet2 - Remote: Spine2 Ethernet4 | PASS | - |
| 182 | Leaf4 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet3 - Remote: Leaf3 Ethernet3 | PASS | - |
| 183 | Leaf4 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet4 - Remote: Leaf3 Ethernet4 | PASS | - |
| 184 | Leaf4 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet5 - Remote: Host-C Ethernet2 | PASS | - |
| 185 | Leaf4 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet6 - Remote: Host-D Ethernet2 | PASS | - |
| 186 | Leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.6) - Destination: Leaf1 Loopback0 (IP: 10.255.0.3) | PASS | - |
| 187 | Leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.6) - Destination: Leaf2 Loopback0 (IP: 10.255.0.4) | PASS | - |
| 188 | Leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.6) - Destination: Leaf3 Loopback0 (IP: 10.255.0.5) | PASS | - |
| 189 | Leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.6) - Destination: Leaf4 Loopback0 (IP: 10.255.0.6) | PASS | - |
| 190 | Leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.6) - Destination: Leaf5 Loopback0 (IP: 10.255.0.7) | PASS | - |
| 191 | Leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.6) - Destination: Leaf6 Loopback0 (IP: 10.255.0.8) | PASS | - |
| 192 | Leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.6) - Destination: Spine1 Loopback0 (IP: 10.255.0.1) | PASS | - |
| 193 | Leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.6) - Destination: Spine2 Loopback0 (IP: 10.255.0.2) | PASS | - |
| 194 | Leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet1 (IP: 10.255.255.13) - Destination: Spine1 Ethernet4 (IP: 10.255.255.12) | PASS | - |
| 195 | Leaf4 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet2 (IP: 10.255.255.15) - Destination: Spine2 Ethernet4 (IP: 10.255.255.14) | PASS | - |
| 196 | Leaf4 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab |
| 197 | Leaf4 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab |
| 198 | Leaf4 | Hardware | VerifyTemperature | Verifies if the device temperature is within acceptable limits. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab |
| 199 | Leaf4 | Hardware | VerifyTransceiversManufacturers | Verifies if all the transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab |
| 200 | Leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet1 - P2P_Spine1_Ethernet4 = 'up' | PASS | - |
| 201 | Leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet2 - P2P_Spine2_Ethernet4 = 'up' | PASS | - |
| 202 | Leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet3 - MLAG_Leaf3_Ethernet3 = 'up' | PASS | - |
| 203 | Leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet4 - MLAG_Leaf3_Ethernet4 = 'up' | PASS | - |
| 204 | Leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet5 - SERVER_Host-C_Ethernet2 = 'up' | PASS | - |
| 205 | Leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet6 - SERVER_Host-D_Ethernet2 = 'up' | PASS | - |
| 206 | Leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback0 - ROUTER_ID = 'up' | PASS | - |
| 207 | Leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback1 - VXLAN_TUNNEL_SOURCE = 'up' | PASS | - |
| 208 | Leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel3 - MLAG_Leaf3_Port-Channel3 = 'up' | PASS | - |
| 209 | Leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel5 - MLAG_PortChannel = 'up' | FAIL | Port-Channel5 - Status mismatch - Expected: up/up, Actual: down/lowerLayerDown |
| 210 | Leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel6 - MLAG_PortChannel = 'up' | FAIL | Port-Channel6 - Status mismatch - Expected: up/up, Actual: down/lowerLayerDown |
| 211 | Leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan21 - VRF_A_VLAN_21 = 'up' | PASS | - |
| 212 | Leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan22 - VRF_A_VLAN_22 = 'up' | PASS | - |
| 213 | Leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan3009 - MLAG_L3_VRF_VRF_A = 'up' | PASS | - |
| 214 | Leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4093 - MLAG_L3 = 'up' | PASS | - |
| 215 | Leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan4094 - MLAG = 'up' | PASS | - |
| 216 | Leaf4 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vxlan1 = 'up' | PASS | - |
| 217 | Leaf4 | MLAG | VerifyMlagStatus | Verifies the health status of the MLAG configuration. | - | PASS | - |
| 218 | Leaf4 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | Routing protocol model: multi-agent | PASS | - |
| 219 | Leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.1 - Peer: Spine1 | PASS | - |
| 220 | Leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.2 - Peer: Spine2 | PASS | - |
| 221 | Leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.3 - Peer: Leaf1 | PASS | - |
| 222 | Leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.4 - Peer: Leaf2 | PASS | - |
| 223 | Leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.5 - Peer: Leaf3 | PASS | - |
| 224 | Leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.6 - Peer: Leaf4 | PASS | - |
| 225 | Leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.7 - Peer: Leaf5 | PASS | - |
| 226 | Leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.8 - Peer: Leaf6 | PASS | - |
| 227 | Leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 192.168.1.3 - Peer: Leaf1 | PASS | - |
| 228 | Leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 192.168.1.5 - Peer: Leaf3 | PASS | - |
| 229 | Leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 192.168.1.7 - Peer: Leaf5 | PASS | - |
| 230 | Leaf4 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 192.168.1.8 - Peer: Leaf6 | PASS | - |
| 231 | Leaf4 | System | VerifyNTP | Verifies if NTP is synchronised. | - | FAIL | NTP status mismatch - Expected: synchronised Actual: NTP is disabled. |
| 232 | Leaf4 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | PASS | - |
| 233 | Leaf5 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: Spine1 (IP: 10.255.0.1) | PASS | - |
| 234 | Leaf5 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: Spine2 (IP: 10.255.0.2) | PASS | - |
| 235 | Leaf5 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: Spine1 (IP: 10.255.255.16) | PASS | - |
| 236 | Leaf5 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: Spine2 (IP: 10.255.255.18) | PASS | - |
| 237 | Leaf5 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet1 - Remote: Spine1 Ethernet5 | PASS | - |
| 238 | Leaf5 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet2 - Remote: Spine2 Ethernet5 | PASS | - |
| 239 | Leaf5 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet5 - Remote: Host-E Ethernet1 | PASS | - |
| 240 | Leaf5 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet6 - Remote: Host-F Ethernet1 | PASS | - |
| 241 | Leaf5 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.7) - Destination: Leaf1 Loopback0 (IP: 10.255.0.3) | PASS | - |
| 242 | Leaf5 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.7) - Destination: Leaf2 Loopback0 (IP: 10.255.0.4) | PASS | - |
| 243 | Leaf5 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.7) - Destination: Leaf3 Loopback0 (IP: 10.255.0.5) | PASS | - |
| 244 | Leaf5 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.7) - Destination: Leaf4 Loopback0 (IP: 10.255.0.6) | PASS | - |
| 245 | Leaf5 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.7) - Destination: Leaf5 Loopback0 (IP: 10.255.0.7) | PASS | - |
| 246 | Leaf5 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.7) - Destination: Leaf6 Loopback0 (IP: 10.255.0.8) | PASS | - |
| 247 | Leaf5 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.7) - Destination: Spine1 Loopback0 (IP: 10.255.0.1) | PASS | - |
| 248 | Leaf5 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.7) - Destination: Spine2 Loopback0 (IP: 10.255.0.2) | PASS | - |
| 249 | Leaf5 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet1 (IP: 10.255.255.17) - Destination: Spine1 Ethernet5 (IP: 10.255.255.16) | PASS | - |
| 250 | Leaf5 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet2 (IP: 10.255.255.19) - Destination: Spine2 Ethernet5 (IP: 10.255.255.18) | PASS | - |
| 251 | Leaf5 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab |
| 252 | Leaf5 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab |
| 253 | Leaf5 | Hardware | VerifyTemperature | Verifies if the device temperature is within acceptable limits. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab |
| 254 | Leaf5 | Hardware | VerifyTransceiversManufacturers | Verifies if all the transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab |
| 255 | Leaf5 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet1 - P2P_Spine1_Ethernet5 = 'up' | PASS | - |
| 256 | Leaf5 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet2 - P2P_Spine2_Ethernet5 = 'up' | PASS | - |
| 257 | Leaf5 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet5 - SERVER_Host-E_Ethernet1 = 'up' | PASS | - |
| 258 | Leaf5 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet6 - SERVER_Host-F_Ethernet1 = 'up' | PASS | - |
| 259 | Leaf5 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback0 - ROUTER_ID = 'up' | PASS | - |
| 260 | Leaf5 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback1 - VXLAN_TUNNEL_SOURCE = 'up' | PASS | - |
| 261 | Leaf5 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel5 - EVPN_AA_PortChannel = 'up' | FAIL | Port-Channel5 - Status mismatch - Expected: up/up, Actual: down/lowerLayerDown |
| 262 | Leaf5 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel6 - EVPN_AA_PortChannel = 'up' | FAIL | Port-Channel6 - Status mismatch - Expected: up/up, Actual: down/lowerLayerDown |
| 263 | Leaf5 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan31 - VRF_A_VLAN_31 = 'up' | PASS | - |
| 264 | Leaf5 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan32 - VRF_A_VLAN_32 = 'up' | PASS | - |
| 265 | Leaf5 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vxlan1 = 'up' | PASS | - |
| 266 | Leaf5 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | Routing protocol model: multi-agent | PASS | - |
| 267 | Leaf5 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.1 - Peer: Spine1 | PASS | - |
| 268 | Leaf5 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.2 - Peer: Spine2 | PASS | - |
| 269 | Leaf5 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.3 - Peer: Leaf1 | PASS | - |
| 270 | Leaf5 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.4 - Peer: Leaf2 | PASS | - |
| 271 | Leaf5 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.5 - Peer: Leaf3 | PASS | - |
| 272 | Leaf5 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.6 - Peer: Leaf4 | PASS | - |
| 273 | Leaf5 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.7 - Peer: Leaf5 | PASS | - |
| 274 | Leaf5 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.8 - Peer: Leaf6 | PASS | - |
| 275 | Leaf5 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 192.168.1.3 - Peer: Leaf1 | PASS | - |
| 276 | Leaf5 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 192.168.1.5 - Peer: Leaf3 | PASS | - |
| 277 | Leaf5 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 192.168.1.7 - Peer: Leaf5 | PASS | - |
| 278 | Leaf5 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 192.168.1.8 - Peer: Leaf6 | PASS | - |
| 279 | Leaf5 | System | VerifyNTP | Verifies if NTP is synchronised. | - | FAIL | NTP status mismatch - Expected: synchronised Actual: NTP is disabled. |
| 280 | Leaf5 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | PASS | - |
| 281 | Leaf6 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: Spine1 (IP: 10.255.0.1) | PASS | - |
| 282 | Leaf6 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: Spine2 (IP: 10.255.0.2) | PASS | - |
| 283 | Leaf6 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: Spine1 (IP: 10.255.255.20) | PASS | - |
| 284 | Leaf6 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: Spine2 (IP: 10.255.255.22) | PASS | - |
| 285 | Leaf6 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet1 - Remote: Spine1 Ethernet6 | PASS | - |
| 286 | Leaf6 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet2 - Remote: Spine2 Ethernet6 | PASS | - |
| 287 | Leaf6 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet5 - Remote: Host-E Ethernet2 | PASS | - |
| 288 | Leaf6 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet6 - Remote: Host-F Ethernet2 | PASS | - |
| 289 | Leaf6 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.8) - Destination: Leaf1 Loopback0 (IP: 10.255.0.3) | PASS | - |
| 290 | Leaf6 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.8) - Destination: Leaf2 Loopback0 (IP: 10.255.0.4) | PASS | - |
| 291 | Leaf6 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.8) - Destination: Leaf3 Loopback0 (IP: 10.255.0.5) | PASS | - |
| 292 | Leaf6 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.8) - Destination: Leaf4 Loopback0 (IP: 10.255.0.6) | PASS | - |
| 293 | Leaf6 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.8) - Destination: Leaf5 Loopback0 (IP: 10.255.0.7) | PASS | - |
| 294 | Leaf6 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.8) - Destination: Leaf6 Loopback0 (IP: 10.255.0.8) | PASS | - |
| 295 | Leaf6 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.8) - Destination: Spine1 Loopback0 (IP: 10.255.0.1) | PASS | - |
| 296 | Leaf6 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: Loopback0 (IP: 10.255.0.8) - Destination: Spine2 Loopback0 (IP: 10.255.0.2) | PASS | - |
| 297 | Leaf6 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet1 (IP: 10.255.255.21) - Destination: Spine1 Ethernet6 (IP: 10.255.255.20) | PASS | - |
| 298 | Leaf6 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet2 (IP: 10.255.255.23) - Destination: Spine2 Ethernet6 (IP: 10.255.255.22) | PASS | - |
| 299 | Leaf6 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab |
| 300 | Leaf6 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab |
| 301 | Leaf6 | Hardware | VerifyTemperature | Verifies if the device temperature is within acceptable limits. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab |
| 302 | Leaf6 | Hardware | VerifyTransceiversManufacturers | Verifies if all the transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab |
| 303 | Leaf6 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet1 - P2P_Spine1_Ethernet6 = 'up' | PASS | - |
| 304 | Leaf6 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet2 - P2P_Spine2_Ethernet6 = 'up' | PASS | - |
| 305 | Leaf6 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet5 - SERVER_Host-E_Ethernet2 = 'up' | PASS | - |
| 306 | Leaf6 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet6 - SERVER_Host-F_Ethernet2 = 'up' | PASS | - |
| 307 | Leaf6 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback0 - ROUTER_ID = 'up' | PASS | - |
| 308 | Leaf6 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback1 - VXLAN_TUNNEL_SOURCE = 'up' | PASS | - |
| 309 | Leaf6 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel5 - EVPN_AA_PortChannel = 'up' | FAIL | Port-Channel5 - Status mismatch - Expected: up/up, Actual: down/lowerLayerDown |
| 310 | Leaf6 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Port-Channel6 - EVPN_AA_PortChannel = 'up' | FAIL | Port-Channel6 - Status mismatch - Expected: up/up, Actual: down/lowerLayerDown |
| 311 | Leaf6 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan31 - VRF_A_VLAN_31 = 'up' | PASS | - |
| 312 | Leaf6 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vlan32 - VRF_A_VLAN_32 = 'up' | PASS | - |
| 313 | Leaf6 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Vxlan1 = 'up' | PASS | - |
| 314 | Leaf6 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | Routing protocol model: multi-agent | PASS | - |
| 315 | Leaf6 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.1 - Peer: Spine1 | PASS | - |
| 316 | Leaf6 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.2 - Peer: Spine2 | PASS | - |
| 317 | Leaf6 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.3 - Peer: Leaf1 | PASS | - |
| 318 | Leaf6 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.4 - Peer: Leaf2 | PASS | - |
| 319 | Leaf6 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.5 - Peer: Leaf3 | PASS | - |
| 320 | Leaf6 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.6 - Peer: Leaf4 | PASS | - |
| 321 | Leaf6 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.7 - Peer: Leaf5 | PASS | - |
| 322 | Leaf6 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 10.255.0.8 - Peer: Leaf6 | PASS | - |
| 323 | Leaf6 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 192.168.1.3 - Peer: Leaf1 | PASS | - |
| 324 | Leaf6 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 192.168.1.5 - Peer: Leaf3 | PASS | - |
| 325 | Leaf6 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 192.168.1.7 - Peer: Leaf5 | PASS | - |
| 326 | Leaf6 | Routing | VerifyRoutingTableEntry | Verifies that the provided routes are present in the routing table of a specified VRF. | Route: 192.168.1.8 - Peer: Leaf6 | PASS | - |
| 327 | Leaf6 | System | VerifyNTP | Verifies if NTP is synchronised. | - | FAIL | NTP status mismatch - Expected: synchronised Actual: NTP is disabled. |
| 328 | Leaf6 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | PASS | - |
| 329 | Spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: Leaf1 (IP: 10.255.0.3) | PASS | - |
| 330 | Spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: Leaf2 (IP: 10.255.0.4) | PASS | - |
| 331 | Spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: Leaf3 (IP: 10.255.0.5) | PASS | - |
| 332 | Spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: Leaf4 (IP: 10.255.0.6) | PASS | - |
| 333 | Spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: Leaf5 (IP: 10.255.0.7) | PASS | - |
| 334 | Spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: Leaf6 (IP: 10.255.0.8) | PASS | - |
| 335 | Spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: Leaf1 (IP: 10.255.255.1) | PASS | - |
| 336 | Spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: Leaf2 (IP: 10.255.255.5) | PASS | - |
| 337 | Spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: Leaf3 (IP: 10.255.255.9) | PASS | - |
| 338 | Spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: Leaf4 (IP: 10.255.255.13) | PASS | - |
| 339 | Spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: Leaf5 (IP: 10.255.255.17) | PASS | - |
| 340 | Spine1 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: Leaf6 (IP: 10.255.255.21) | PASS | - |
| 341 | Spine1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet1 - Remote: Leaf1 Ethernet1 | PASS | - |
| 342 | Spine1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet2 - Remote: Leaf2 Ethernet1 | PASS | - |
| 343 | Spine1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet3 - Remote: Leaf3 Ethernet1 | PASS | - |
| 344 | Spine1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet4 - Remote: Leaf4 Ethernet1 | PASS | - |
| 345 | Spine1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet5 - Remote: Leaf5 Ethernet1 | PASS | - |
| 346 | Spine1 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet6 - Remote: Leaf6 Ethernet1 | PASS | - |
| 347 | Spine1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet1 (IP: 10.255.255.0) - Destination: Leaf1 Ethernet1 (IP: 10.255.255.1) | PASS | - |
| 348 | Spine1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet2 (IP: 10.255.255.4) - Destination: Leaf2 Ethernet1 (IP: 10.255.255.5) | PASS | - |
| 349 | Spine1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet3 (IP: 10.255.255.8) - Destination: Leaf3 Ethernet1 (IP: 10.255.255.9) | PASS | - |
| 350 | Spine1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet4 (IP: 10.255.255.12) - Destination: Leaf4 Ethernet1 (IP: 10.255.255.13) | PASS | - |
| 351 | Spine1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet5 (IP: 10.255.255.16) - Destination: Leaf5 Ethernet1 (IP: 10.255.255.17) | PASS | - |
| 352 | Spine1 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet6 (IP: 10.255.255.20) - Destination: Leaf6 Ethernet1 (IP: 10.255.255.21) | PASS | - |
| 353 | Spine1 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab |
| 354 | Spine1 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab |
| 355 | Spine1 | Hardware | VerifyTemperature | Verifies if the device temperature is within acceptable limits. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab |
| 356 | Spine1 | Hardware | VerifyTransceiversManufacturers | Verifies if all the transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab |
| 357 | Spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet1 - P2P_Leaf1_Ethernet1 = 'up' | PASS | - |
| 358 | Spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet2 - P2P_Leaf2_Ethernet1 = 'up' | PASS | - |
| 359 | Spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet3 - P2P_Leaf3_Ethernet1 = 'up' | PASS | - |
| 360 | Spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet4 - P2P_Leaf4_Ethernet1 = 'up' | PASS | - |
| 361 | Spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet5 - P2P_Leaf5_Ethernet1 = 'up' | PASS | - |
| 362 | Spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet6 - P2P_Leaf6_Ethernet1 = 'up' | PASS | - |
| 363 | Spine1 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback0 - ROUTER_ID = 'up' | PASS | - |
| 364 | Spine1 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | Routing protocol model: multi-agent | PASS | - |
| 365 | Spine1 | System | VerifyNTP | Verifies if NTP is synchronised. | - | FAIL | NTP status mismatch - Expected: synchronised Actual: NTP is disabled. |
| 366 | Spine1 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | PASS | - |
| 367 | Spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: Leaf1 (IP: 10.255.0.3) | PASS | - |
| 368 | Spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: Leaf2 (IP: 10.255.0.4) | PASS | - |
| 369 | Spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: Leaf3 (IP: 10.255.0.5) | PASS | - |
| 370 | Spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: Leaf4 (IP: 10.255.0.6) | PASS | - |
| 371 | Spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: Leaf5 (IP: 10.255.0.7) | PASS | - |
| 372 | Spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP EVPN Peer: Leaf6 (IP: 10.255.0.8) | PASS | - |
| 373 | Spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: Leaf1 (IP: 10.255.255.3) | PASS | - |
| 374 | Spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: Leaf2 (IP: 10.255.255.7) | PASS | - |
| 375 | Spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: Leaf3 (IP: 10.255.255.11) | PASS | - |
| 376 | Spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: Leaf4 (IP: 10.255.255.15) | PASS | - |
| 377 | Spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: Leaf5 (IP: 10.255.255.19) | PASS | - |
| 378 | Spine2 | BGP | VerifyBGPSpecificPeers | Verifies the health of specific BGP peer(s) for given address families. | BGP IPv4 Unicast Peer: Leaf6 (IP: 10.255.255.23) | PASS | - |
| 379 | Spine2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet1 - Remote: Leaf1 Ethernet2 | PASS | - |
| 380 | Spine2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet2 - Remote: Leaf2 Ethernet2 | PASS | - |
| 381 | Spine2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet3 - Remote: Leaf3 Ethernet2 | PASS | - |
| 382 | Spine2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet4 - Remote: Leaf4 Ethernet2 | PASS | - |
| 383 | Spine2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet5 - Remote: Leaf5 Ethernet2 | PASS | - |
| 384 | Spine2 | Connectivity | VerifyLLDPNeighbors | Verifies the connection status of the specified LLDP (Link Layer Discovery Protocol) neighbors. | Local: Ethernet6 - Remote: Leaf6 Ethernet2 | PASS | - |
| 385 | Spine2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet1 (IP: 10.255.255.2) - Destination: Leaf1 Ethernet2 (IP: 10.255.255.3) | PASS | - |
| 386 | Spine2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet2 (IP: 10.255.255.6) - Destination: Leaf2 Ethernet2 (IP: 10.255.255.7) | PASS | - |
| 387 | Spine2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet3 (IP: 10.255.255.10) - Destination: Leaf3 Ethernet2 (IP: 10.255.255.11) | PASS | - |
| 388 | Spine2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet4 (IP: 10.255.255.14) - Destination: Leaf4 Ethernet2 (IP: 10.255.255.15) | PASS | - |
| 389 | Spine2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet5 (IP: 10.255.255.18) - Destination: Leaf5 Ethernet2 (IP: 10.255.255.19) | PASS | - |
| 390 | Spine2 | Connectivity | VerifyReachability | Test network reachability to one or many destination IP(s). | Source: P2P Interface Ethernet6 (IP: 10.255.255.22) - Destination: Leaf6 Ethernet2 (IP: 10.255.255.23) | PASS | - |
| 391 | Spine2 | Hardware | VerifyEnvironmentCooling | Verifies the status of power supply fans and all fan trays. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentCooling test is not supported on cEOSLab |
| 392 | Spine2 | Hardware | VerifyEnvironmentPower | Verifies the power supplies status. | Accepted States: 'ok' | SKIPPED | VerifyEnvironmentPower test is not supported on cEOSLab |
| 393 | Spine2 | Hardware | VerifyTemperature | Verifies if the device temperature is within acceptable limits. | - | SKIPPED | VerifyTemperature test is not supported on cEOSLab |
| 394 | Spine2 | Hardware | VerifyTransceiversManufacturers | Verifies if all the transceivers come from approved manufacturers. | Accepted Manufacturers: 'Arista Networks', 'Arastra, Inc.', 'Not Present' | SKIPPED | VerifyTransceiversManufacturers test is not supported on cEOSLab |
| 395 | Spine2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet1 - P2P_Leaf1_Ethernet2 = 'up' | PASS | - |
| 396 | Spine2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet2 - P2P_Leaf2_Ethernet2 = 'up' | PASS | - |
| 397 | Spine2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet3 - P2P_Leaf3_Ethernet2 = 'up' | PASS | - |
| 398 | Spine2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet4 - P2P_Leaf4_Ethernet2 = 'up' | PASS | - |
| 399 | Spine2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet5 - P2P_Leaf5_Ethernet2 = 'up' | PASS | - |
| 400 | Spine2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Ethernet6 - P2P_Leaf6_Ethernet2 = 'up' | PASS | - |
| 401 | Spine2 | Interfaces | VerifyInterfacesStatus | Verifies the operational states of specified interfaces to ensure they match expected configurations. | Interface Loopback0 - ROUTER_ID = 'up' | PASS | - |
| 402 | Spine2 | Routing | VerifyRoutingProtocolModel | Verifies the configured routing protocol model. | Routing protocol model: multi-agent | PASS | - |
| 403 | Spine2 | System | VerifyNTP | Verifies if NTP is synchronised. | - | FAIL | NTP status mismatch - Expected: synchronised Actual: NTP is disabled. |
| 404 | Spine2 | System | VerifyReloadCause | Verifies the last reload cause of the device. | - | PASS | - |
