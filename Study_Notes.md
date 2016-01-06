This is a repository to track my preparation for the ONF Certified Associate Certification. The Blue Print is obtained from the ONF site and for authoritative and updated topics, kindly visit https://www.opennetworking.org/skills-associate#examblueprint. The material is from a variety of sites online, youtube videos and SDN books. As much as I can, I will be linking the source of the materials. Any omission is not deliberate and I will endeavour to cite as many sources as possible.

## ONF Certified SDN Associate Examination Blueprint


### Domain	 	% Weight of Exam (40 questions from random pool)

 	 	 
1. Networking Concepts	 	15%
2. SDN Concepts	 	25%
3. OpenFlow	 	25%
4. SDN Architecture and Ecosystem	 	25%
5. SDN Open Source	 	10%
 
##### DOMAIN 1: NETWORKING CONCEPTS 15%
_Identify and compare the layers of OSI and TCP/IP models and functionality of various fundamental elements of networking._
  * OSI Model - ISO/IEC 7498-1: a standard of the International Organization for Standardization (ISO). It is a general-purpose paradigm for discussing or describing how computers communicate with one another over a network. Its seven-layered approach to data transmission divides the many operations up into specific related groups of actions at each layer 
1. OSI and TCP/IP Comparison.

    <table>
      <tr><center>
        <td><b>OSI</b></td>
        <td><b>TCP/IP</b></td>
        </center>
      </tr>
    
      <tr>
        <td>Application</td>
        <td rowspan = "3">Application</td>
      </tr>
      
      <tr>
        <td>Presentation</td>
      </tr>
      
      <tr>
        <td>Session&nbsp;</td>
      </tr>
    
      <tr>
        <td>Transport</td>
        <td>Transport</td>
      </tr>
    
      <tr>
        <td>Network</td>
        <td>Internet</td>
      </tr>
    
      <tr>
        <td>Data Link</td>
        <td rowspan = "2">Network Access</td>
      </tr>
    
      <tr>
        <td>Physical&nbsp;</td>
      </tr>
    </table>
_From [studytonight] (http://www.studytonight.com/computer-networks/comparison-osi-tcp-model), following are some major differences between OSI Reference Model and TCP/IP Reference Model, with diagrammatic comparison below._
    <table>
       <tr>
         <td><b>OSI (Open System Interconnection)</b></td>
         <td><b>TCP/IP (Transmission Control Protocol / Internet Protocol)</b></td>
       </tr>
       
       <tr>
         <td>1. OSI provides layer functioning and also defines functions of all the layers.</td>	
         <td>1. TCP/IP model is more based on protocols and protocols are not flexible with other layers.</td>
       </tr>
       
       <tr>
         <td>2. In OSI model the transport layer guarantees the delivery of packets</td>	
         <td>2. In TCP/IP model the transport layer does not guarantees delivery of packets.</td>
       </tr>
     
       <tr>
         <td>3. Follows horizontal approach</td>	
         <td>3. Follows vertical approach.</td>
       </tr>
  
       <tr>
          <td>4. OSI model has a separate presentation layer</td>	
          <td>4. TCP/IP does not have a separate presentation layer</td>
       </tr>
       
       <tr>
          <td>5. OSI is a general model.</td>	
          <td>5. TCP/IP model cannot be used in any other application.</td>
       </tr>
       
       <tr>
          <td>6. Network layer of OSI model provide both connection oriented and connectionless service.	
          <td>6. The Network layer in TCP/IP model provides connectionless service.</td>
       </tr>
       
       <tr>
          <td>7. OSI model has a problem of fitting the protocols in the model</td>	
          <td>7. TCP/IP model does not fit any protocol</td>
       </tr>
       
       <tr>
          <td>8. Protocols are hidden in OSI model and are easily replaced as the technology changes.</td>	
          <td>8. In TCP/IP replacing protocol is not easy.</td>
       </tr>
       
       <tr>
          <td>9. OSI model defines services, interfaces and protocols very clearly and makes clear distinction between them.</td>	
          <td>9. In TCP/IP it is not clearly separated its services, interfaces and protocols.</td>
       </tr>
       
       <tr>
          <td>10. It has 7 layers</td>	10. 
          <td>10. It has 4 layers</td>
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
1. Describe the fundamental characteristics of SDN, definitions, use cases, and history.
  * Alpha
  * Bravo
2. History of SDN (Clean Slate, Ethane, OpenFlow®, donation to ONF)
  * Alpha
  * Bravo
3. What is SDN? (control and forwarding)
  * Alpha
  * Bravo
4. SDN Value Proposition
  * Alpha
  * Bravo
5. SDN Use Cases in the Data Center
  * Alpha
  * Bravo
6. SDN Use Cases in Campus Networks
  * Alpha
  * Bravo
7. SDN Use Cases in Service Providers
  * Alpha
  * Bravo
8. SDN Use Cases in the Enterprise
  * Alpha
  * Bravo
9. SDN Use Cases in Mobile Networks
  * Alpha
  * Bravo
10. The six characteristics of an SDN Network (Plane Separation, Simplified Forwarding Element, Centralized Control, Network Automation, Virtualization, and Openness)
  * Alpha
  * Bravo
11. SDN Devices (Controllers, Switches, Orchestration, API's)
  * Alpha
  * Bravo
12. Overlay Networking Abstractions (NFV, VxLAN, etc.)
  * Alpha
  * Bravo
 
### DOMAIN 3: OPENFLOW® 25%
13. Identify at a concept/definition level the OpenFlow® Protocol operations and list the packet types and contents.
  * Alpha
  * Bravo
14. TCP level secure channel/communication/session establishment between controller/switch
  * Alpha
  * Bravo
15. Message Types
  * Alpha
  * Bravo
16. Basic Operation/Packet Matching
  * Alpha
  * Bravo
17. Differences between OpenFlow® versions
  * Alpha
  * Bravo
18. Proactive vs Reactive Flows
  * Alpha
  * Bravo
19. Statistics/Counters
  * Alpha
  * Bravo
20. Setting up a flow
  * Alpha
  * Bravo
21. Policy Enforcement
  * Alpha
  * Bravo
22. OpenFlow® Management and Configuration Protocol (OF-Config, OAM, OFDPA, OVSDB, etc.)
  * Alpha
  * Bravo
23. Flow Table Entry Format
  * Alpha
  * Bravo
24. Flow Timers
  * Alpha
  * Bravo
25. Pipeline Processing
  * Alpha
  * Bravo
26. Match Types
  * Alpha
  * Bravo
27. Match Actions
  * Alpha
  * Bravo
 
### DOMAIN 4: SDN ARCHITECTURE AND ECOSYSTEM 25%
1. Understand and Identify SDN architectural components, standards bodies, controller design, API’s and applications.
  * Alpha
  * Bravo
2. SDN Layers
  * Alpha
  * Bravo
3. SDN Architecture compared to Traditional Network Architectures
  * Alpha
  * Bravo
4. Northbound API's
  * Alpha
  * Bravo
5. Southbound API's
  * Alpha
  * Bravo
6. East/West API's
  * Alpha
  * Bravo
7. Security and Availability
  * Alpha
  * Bravo
8. Packet and Optical Integration methods
  * Alpha
  * Bravo
9. Migration Strategies
  * Alpha
  * Bravo
10. Hybrid Mode Switches
  * Alpha
  * Bravo
11. Organization in the SDN Ecosystem
  * Alpha
  * Bravo
12. Standards Bodies and Industry alliances
  * Alpha
  * Bravo
13. Network Operators and Enterprises
  * Alpha
  * Bravo
14. Network Equipment Manufacturers
  * Alpha
  * Bravo
15. Software vendors
  * Alpha
  * Bravo
16. Academic and Industry research institutions and labs
  * Alpha
  * Bravo
17. Open Source Initiatives
  * Alpha
  * Bravo
18. Who is the ONF and what do they do?
  * Alpha
  * Bravo
19. Purpose
  * Alpha
  * Bravo
20. Structure
  * Alpha
  * Bravo
21. Technical Working Groups
  * Alpha
  * Bravo
22. Open Source Software Development
  * Alpha
  * Bravo
23. Activities and Initiatives
  * Alpha
  * Bravo
24. Controller Placement and Redundancy
  * Alpha
  * Bravo
25. SDN Applications (service chaining, virtualized network functions, analytics)
  * Alpha
  * Bravo
 
### DOMAIN 5: OPEN SOURCE SDN 10%
1. Identify key open source projects in the SDN Ecosystem.
  * Alpha
  * Bravo
2. OpenFlow® Agents
  * Alpha
  * Bravo
3. Indigo
  * Alpha
  * Bravo
4. Linc
  * Alpha
  * Bravo
5. OVS
  * Alpha
  * Bravo
6. CPqD/ONF Driver (aka "libFluid")
  * Alpha
  * Bravo
7. OpenFlow® Controllers
  * Alpha
  * Bravo
8. NOX
  * Alpha
  * Bravo
9. POX
  * Alpha
  * Bravo
10. ONOS
  * Alpha
  * Bravo
11. ODL
  * Alpha
  * Bravo
12. Floodlight
  * Alpha
  * Bravo
13. RYU
  * Alpha
  * Bravo
14. Utilities and Tools
  * Alpha
  * Bravo
15. FlowSim
  * Alpha
  * Bravo
16. Mininet
  * Alpha
  * Bravo
17. Of DPA
  * Alpha
  * Bravo
18. OF Test
  * Alpha
  * Bravo
19. Wireshark
  * Alpha
  * Bravo
20. Avior
  * Alpha
  * Bravo
21. Open Source SDN Distributions (OSSDN Atrium, etc.)
  * Alpha
  * Bravo
22. Open vSwitch
  * Alpha
  * Bravo
23. Orchestration Systems
  * Alpha
  * Bravo
24. Open Source Initiatives (OPNFV, OCP, ODCA, Open Config)
  * Alpha
  * Bravo
