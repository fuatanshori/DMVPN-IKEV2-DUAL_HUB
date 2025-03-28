# DMVPN Dual Hub Phase 3 with IKEv2 Configuration

## Network Topology
![DMVPN Topology](/file/topologi.png)

## Overview
This repository contains the configuration for a Dynamic Multipoint VPN (DMVPN) network with the following key characteristics:
- Dual Hub topology (HUB-1 and HUB-2)
- DMVPN Phase 3
- IKEv2 authentication
- Spoke-and-hub design with multiple spoke sites

## Network Components
- **Hubs**: HUB-1 (192.168.0.0/24), HUB-2 (192.168.50.0/24)
- **Spokes**: 
  - SPOKE-1 (192.168.150.0/24)
  - SPOKE-2 (192.168.200.0/24)
  - SPOKE-3 (192.168.250.0/24)
  - SPOKE-4 (192.168.254.0/24)
- **Switches**: SW1, SW2, SW3, SW4, SW5

## Key Configuration Features
- DMVPN Phase 3 allows dynamic spoke-to-spoke tunneling
- IKEv2 for enhanced security and authentication
- Dynamic routing support

## Prerequisites
- Cisco IOS devices supporting DMVPN Phase 3
- IKEv2 capability
- OSPF for dynamic routing
- IPsec for tunnel encryption

## Configuration Steps
1. Configure IKEv2 authentication
2. Set up DMVPN tunnel interfaces
3. Configure IPsec protection
4. Implement dynamic routing


## Recommended Security Measures
- Use strong authentication methods
- Implement IPsec encryption
- Use access lists to control traffic

## Troubleshooting
- Verify tunnel connectivity
- Check IKEv2 negotiation
- Monitor routing tables


## License
This project is licensed under the MIT License - see the LICENSE.md file for details.

## Router Version
- Vios-adventerprisek9-m.SPA.159.M6