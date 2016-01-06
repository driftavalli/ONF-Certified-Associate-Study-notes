This is a repository to track my preparation for the ONF Certified Associate Certification. The Blue Print is obtained from the ONF site and for authoritative and updated topics, kindly visit https://www.opennetworking.org/skills-associate#examblueprint. The material is from a variety of sites online, youtube videos and SDN books. As much as I can, I will be linking the source of the materials. Any omission is not deliberate and I will endeavour to cite as many sources as possible.

## ONF Certified SDN Associate Examination Blueprint


### Domain	 	% Weight of Exam (40 questions from random pool)

 	 	 
1. Networking Concepts	 	15%
2. SDN Concepts	 	25%
3. OpenFlow	 	25%
4. SDN Architecture and Ecosystem	 	25%
5. SDN Open Source	 	10%
 
##### DOMAIN 1: NETWORKING CONCEPTS 15%
1. Identify and compare the layers of OSI and TCP/IP models and functionality of various fundamental elements of networking.
  * Alpha
  * Bravo
2. OSI and TCP/IP Comparison.

    <table>
      <tr><center>
        <td><b>OSI</b></td>
        <td><b>TCP/IP</b></td>
        <td><b>Comparison</b></td>
      </center></tr>
    
      <tr>
        <td>Application</td>
        <td rowspan = "3">Application</td>
        <td></td>
      </tr>
      
      <tr>
        <td>Presentation&nbsp;</td>
        <td>&nbsp;</td>
      </tr>
      
      <tr>
        <td>Session&nbsp;</td>
        <td>&nbsp;</td>
      </tr>
    
      <tr>
        <td>Transport&nbsp;</td>
        <td>Transport&nbsp;</td>
        <td>&nbsp;</td>
      </tr>
    
      <tr>
        <td>Network&nbsp;</td>
        <td>Internet&nbsp;</td>
        <td>&nbsp;</td>
      </tr>
    
      <tr>
        <td>Data Link&nbsp;</td>
        <td rowspan = "2">Network Access&nbsp;</td>
        <td>&nbsp;</td>
      </tr>
    
      <tr>
        <td>Physical&nbsp;</td>
        <td>&nbsp;</td>
      </tr>
    </table>

3. Ethernet networks
  * Alpha
  * Bravo
4. Collision domains and broadcast domains
  * Alpha
  * Bravo
5. Function of routers and switches
  * Alpha
  * Bravo
6. Routing Protocols (RIP, OSPF, ISIS, BGP)
  * Alpha
  * Bravo
7. Optical network fundamentals – SONET/SDH, OTN
  * Alpha
  * Bravo
8. IP Network Services ( DHCP, DNS, ARP, NAT, ICMP)
  * Alpha
  * Bravo
9. Layer 2 addressing, including address resolution
  * Alpha
  * Bravo
10. IPv4 and IPv6 fundamentals
  * Alpha
  * Bravo
11. Layer 3 / IP addressing, including subnet masks
  * Alpha
  * Bravo
12. Longest match routing
  * Alpha
  * Bravo
13. Connection-oriented vs. connectionless protocols
  * Alpha
  * Bravo
14. Packet Filtering with Match/Action Pairs
  * Alpha
  * Bravo

  
  

### DOMAIN 2: SDN CONCEPTS 25%
Describe the fundamental characteristics of SDN, definitions, use cases, and history.
History of SDN (Clean Slate, Ethane, OpenFlow®, donation to ONF)
What is SDN? (control and forwarding)
SDN Value Proposition
SDN Use Cases in the Data Center
SDN Use Cases in Campus Networks
SDN Use Cases in Service Providers
SDN Use Cases in the Enterprise
SDN Use Cases in Mobile Networks
The six characteristics of an SDN Network (Plane Separation, Simplified Forwarding Element, Centralized Control, Network Automation, Virtualization, and Openness)
SDN Devices (Controllers, Switches, Orchestration, API's)
Overlay Networking Abstractions (NFV, VxLAN, etc.)
 
### DOMAIN 3: OPENFLOW® 25%
Identify at a concept/definition level the OpenFlow® Protocol operations and list the packet types and contents.
TCP level secure channel/communication/session establishment between controller/switch
Message Types
Basic Operation/Packet Matching
Differences between OpenFlow® versions
Proactive vs Reactive Flows
Statistics/Counters
Setting up a flow
Policy Enforcement
OpenFlow® Management and Configuration Protocol (OF-Config, OAM, OFDPA, OVSDB, etc.)
Flow Table Entry Format
Flow Timers
Pipeline Processing
Match Types
Match Actions
 
### DOMAIN 4: SDN ARCHITECTURE AND ECOSYSTEM 25%
Understand and Identify SDN architectural components, standards bodies, controller design, API’s and applications.
SDN Layers
SDN Architecture compared to Traditional Network Architectures
Northbound API's
Southbound API's
East/West API's
Security and Availability
Packet and Optical Integration methods
Migration Strategies
Hybrid Mode Switches
Organization in the SDN Ecosystem
Standards Bodies and Industry alliances
Network Operators and Enterprises
Network Equipment Manufacturers
Software vendors
Academic and Industry research institutions and labs
Open Source Initiatives
Who is the ONF and what do they do?
Purpose
Structure
Technical Working Groups
Open Source Software Development
Activities and Initiatives
Controller Placement and Redundancy
SDN Applications (service chaining, virtualized network functions, analytics)
 
### DOMAIN 5: OPEN SOURCE SDN 10%
Identify key open source projects in the SDN Ecosystem.
OpenFlow® Agents
Indigo
Linc
OVS
CPqD/ONF Driver (aka "libFluid")
OpenFlow® Controllers
NOX
POX
ONOS
ODL
Floodlight
RYU
Utilities and Tools
FlowSim
Mininet
Of DPA
OF Test
Wireshark
Avior
Open Source SDN Distributions (OSSDN Atrium, etc.)
Open vSwitch
Orchestration Systems
Open Source Initiatives (OPNFV, OCP, ODCA, Open Config)
