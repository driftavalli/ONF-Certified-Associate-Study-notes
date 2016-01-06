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
  * OSI Model - ISO/IEC 7498-1: a standard of the International Organization for Standardization (ISO). Used for describing how computers communicate with one another over a network. It divides communication and data transmission between two compute nodes into seven layers with each layer responsible for specific functions and relies on the underlying layer for other needed services.
  * TCP/IP Model - : most widely used protocol suite. "[TCP/IP] (https://technet.microsoft.com/en-ca/library/cc786128%28v=ws.10%29.aspx?f=255&MSPPError=-2147217396) protocols map to a four-layer conceptual model known as the DARPA model, named after the U.S. government agency that initially developed TCP/IP. The four layers of the DARPA model are: Application, Transport, Internet, and Network Interface. Each layer in the DARPA model corresponds to one or more layers of the seven-layer Open Systems Interconnection (OSI) model." There is an TCP/IP tutoria [here] (). A [list](https://technet.microsoft.com/en-ca/library/cc737968(v=ws.10).aspx) of some TCP/IP _rfcs_ include: [768 - User Datagram Protocol (UDP)] (), [783 - Trivial File Transfer Protocol (TFTP)] (), [791 - Internet Protocol (IP)] (), [792 - Internet Control Message Protocol (ICMP)] (), [793 - Transmission Control Protocol (TCP)] (), [826 - Address Resolution Protocol (ARP)] (), [854 - Telnet Protocol (TELNET)] (), [862 - Echo Protocol (ECHO)] (), [959 - File Transfer Protocol (FTP)] (), [1112 - Internet Group Management Protocol (IGMP)] (), [115 - Simple Network Management Protocol (SNMP)] (), [2131 - Dynamic Host Configuration Protocol (DHCP)] (), [2236 - Internet Group Management Protocol, Version 2] (). 

  * A very good resource is the [The TCP/IP Guide] (http://www.tcpipguide.com/index.htm) site, which provides a comprehensive study of the suite.

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
  * [Wikipedia] (https://en.wikipedia.org/wiki/Ethernet) has a pretty comprehensive article on ethernet; _"Ethernet /ˈiːθərnɛt/ is a family of computer networking technologies for local area networks (LANs) and metropolitan area networks (MANs). It was commercially introduced in 1980 and first standardized in 1983 as IEEE 802.3,[1] and has since been refined to support higher bit rates and longer link distances. Over time, Ethernet has largely replaced competing wired LAN technologies such as token ring, FDDI, and ARCNET."_
  * If you want a peek at the actual standards, the [IEEE] (https://www.ieee.org/) provides free downloads of the standards through their [Get Program] (https://standards.ieee.org/about/get/802/802.3.html).
  * [Cisco] (www.cisco.com) also has a pretty decent book on the Ethernet standards. Access it [here] (http://www.cisco.com/c/en/us/td/docs/net_mgmt/active_network_abstraction/3-7/reference/guide/ANARefGuide37/ethrnt.html)
4. Collision domains and broadcast domains: 
   Any decent entry level certification study guide should have materials on both of these topics. 	
   
   A collision domain is a part of a network where packet collisions can occur  (OSI layer 1).  A broadcast domain contains all devices that can reach each other at the data link layer (OSI layer 2) by using a broadcast. A collision domain would be created by a hub while a broadcast domain would be created by a switch. Routers do not forward broadcasts hence the separate broadcast domains.
   
   I have also added a variety of sources found online.
  * Collision domains: [Wikipedia] (https://en.wikipedia.org/wiki/Collision_domain) to the rescue again: _"A collision domain is a section of a network connected by a shared medium or through repeaters where data packets can collide with one another when being sent, particularly when using early versions of Ethernet. A network collision occurs when more than one device attempts to send a packet on a network segment at the same time."_ See also Cisco's [learning network] (https://learningnetwork.cisco.com/thread/1734). See also [Study CCNA] (http://study-ccna.com/collision-broadcast-domain) for another good explanation.
  * Broadcast domains: From [Wikipedia] (https://en.wikipedia.org/wiki/Broadcast_domain): _"A broadcast domain is a logical division of a computer network, in which all nodes can reach each other by broadcast at the data link layer. A broadcast domain can be within the same LAN segment or it can be bridged to other LAN segments."_
 
5. Function of routers and switches
  * Switches create a network. A network switch connects multiple computers together within one local area network (LAN).
  * Routers connect networks. A router links computers /resources in one network to resources in a different network. A router acts as a dispatcher, choosing the best path for information to travel so it's received quickly. Additional material can be found [here - Nutt.net] (http://www.nutt.net/2004/11/20/difference-in-hub-switch-bridge-router/).
  
6. Routing Protocols (RIP, OSPF, ISIS, BGP)
  * Alpha
  * Bravo
7. Optical network fundamentals – SONET/SDH, OTN
  ######SONET/SDH:
SONET is a set of standards that define the rates and formats for optical networks specified in ANSI. A similar standard, Synchronous Digital Hierarchy (SDH), is specified by the International Telecommunication Union Telecommunication Standardization Sector (ITU-T).  SONET equipment is generally used in North America, and SDH equipment generally in the rest of the world. SONET defines optical carrier (OC) levels, electrically equivalent synchronous transport signals (STSs/STMs) and a synchronous frame structure for multiplexed digital traffic for the fiber-optic based transmission hierarchy. The SONET standard includes four  functional layers: the photonic, the section, the line, and the path layer. They correspond to both the physical and the data link layers.
 * Photonic: This refers to the actual physical fibre-optic cable.
 * Section: A section is a single fiber run that can be terminated by a network element (Line or Path) or an optical regenerator. The main function of the section layer is to properly format the SONET frames, and to convert the electrical signals to optical signals. Section Terminating Equipment (STE) can originate, access, modify, or terminate the section header overhead. A SONET STS-n signal is transmitted at 8000 frames per second (A standard STS-1 frame is nine rows by 90 bytes). Each byte in a SONET frame can carry a digitized voice channel. The first three bytes of each row comprise the Section and Line header overhead.
 * Line: Line-Terminating Equipment (LTE) originates or terminates one or more sections of a line signal. The LTE does the synchronization and multiplexing of information on SONET frames. Multiple lower-level SONET signals can be mixed together to form higher-level SONET signals. An Add/Drop Multiplexer (ADM) is an example of LTE.
 * Path:Path-Terminating Equipment (PTE) interfaces non-SONET equipment to the SONET network. At this layer, the payload is mapped and de-mapped into the SONET frame. For example, an STS PTE can assemble 25 1.544 Mbps DS1 signals and insert path overhead to form an STS-1 signal. This layer is concerned with end-to-end transport of data.
			The first 3 columns of SONET frame are called Transport Overhead (TOH). The remaining 87 columns are called Synchronous Payload Envelope (SPE). The first column of SPE is called Payload Overhead (POH).In SONET, the data rate of an STS-n signal is n times the data rate of an STS-1 signal and the duration of any frame is 125us. Transport is achieved in SONET by packaging signals into containers. Section overheads are then added so that the signal and the quality of transmission are all traceable. The containers have two names depending on size: virtual tributary (VT) or a synchronous payload envelope (SPE). The path overhead contains data to control the facility (end to end) such as for path trace, error monitoring, far-end error, or virtual container (VC) composition. 

  * 
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

1. History of SDN (Clean Slate, Ethane, OpenFlow®, donation to ONF)
  * Alpha
  * Bravo
2. What is SDN? (control and forwarding)
  * Alpha
  * Bravo
3. SDN Value Proposition
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
