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
  * Clean Slate project: program that sought to reimagine how networks were built and the underlying protocols. Had several programs at Stanford and Princeton universities.
  * Ethane Project came out of Stanford and …
  * OpenFlow was also primarily from Stanford and …
  * Control and management of the OpenFlow protocol was handed over to ONF …

 
2. What is SDN? (control and forwarding)
  The [ONF defines SDN] (https://www.opennetworking.org/sdn-resources/sdn-definition) as "the physical separation of the network control plane from the forwarding plane, and where a control plane controls several devices. 
  * Software-Defined Networking (SDN) is an emerging architecture that is dynamic, manageable, cost-effective, and adaptable, making it ideal for the high-bandwidth, dynamic nature of today's applications. This architecture decouples the network control and forwarding functions enabling the network control to become directly programmable and the underlying infrastructure to be abstracted for applications and network services. The OpenFlow® protocol is a foundational element for building SDN solutions.
  * The SDN architecture is:
	  1. Directly programmable: Network control is directly programmable because it is decoupled from forwarding functions.
	  2. Agile: Abstracting control from forwarding lets administrators dynamically adjust network-wide traffic flow to meet changing needs.
	  3. Centrally managed: Network intelligence is (logically) centralized in software-based SDN controllers that maintain a global view of the network, which appears to applications and policy engines as a single, logical switch.
	  4. Programmatically configured: SDN lets network managers configure, manage, secure, and optimize network resources very quickly via dynamic, automated SDN programs, which they can write themselves because the programs do not depend on proprietary software.
	  5. Open standards-based and vendor-neutral: When implemented through open standards, SDN simplifies network design and operation because instructions are provided by SDN controllers instead of multiple, vendor-specific devices and protocols."


3. SDN Value Proposition
  * Application/service enablement: The potential of layered applications that could control, coordinate and redefine the network to support new “value add” services will lead to reduced cycle time for introduction of new services as well as reduced cycle time to remove old or poor services.
  * Reduced operational and total cost of ownership/Increased operational efficiencies: By implementing a more intelligent framework that abstracts the network allowing simplification of time consuming, or difficult operational tasks.
  * Hardware simplification /flexibility: Differentiating network functionality in the software domain makes generic hardware possible and allows more resource pooling and functional flexibility. The composition or decomposition of functions allows more flexibility in responding to the market as well as allowing the creation of APIs much more quickly. This enables cost reduction based upon functional reallocation and resource scaling.

5. SDN Use Cases in the Data Center
  * Traffic Engineering
  * Quality of Service
  * Greater Link Loading/Utilization
  * Virtual machine migration.
  * Service chaining.
  * Security services.
  * Load balancer services.
  * Software defined clouds.
  * Cloud hosting.

6. SDN Use Cases in Campus Networks
  * Dynamic QoS and traffic engineering.
  * Unified wired and wireless networks.
  * QoS management for VoIP across wired and wireless networks.
  * Role based access.

7. SDN Use Cases in Service Providers
  * Network Access Control: Provides the ability to set appropriate privileges/access control limits for users/devices accessing the networks, while incorporating service chains as well as quality of service. Also allows policy to follow the user/device as they connect from different parts of the network. 
  * Network Virtualization: Allows the creation of an abstracted virtual network on top of a physical network, allowing a large number of multi-tenant networks to run over a physical network, spanning multiple racks in the datacenter or locations if necessary, including fine-grained controls and isolation as well as insertion of acceleration or security services.
  * Mobility Virtualization: Virtual CPE and Service Chaining.
  * NFV and Service Orchestration: Ability to provide a better way of operating in a hybrid, physical/virtual environment through orchestration. This allows the combination of virtual and physical networking functions such that the full benefits of the infrastructure is realized and thereby improve service delivery to end users.
WAN Optimization & Innovation: The use of SDN through NfV reduces network complexity and leads to simpler network designs. This allows better visibility of the network which leads to better traffic engineering. A holistic view of the network across different transport and IP network layers can allow dynamic bandwidth optimization which reduces cost and is more responsive to business needs. An SDN controller can apply policy dynamically to improve the customer experience without over-provisioning.
  * Policy Driven Application Provisioning & Delivery: Data center application delivery can a competitive advantage if done reliably and successfully. Eliminating the manual process of provisioning and delivering applications into a simplified, automated, policy-driven process can yield significant cost savings, as well as improvements in security compliance and customer experience. The ability to apply policies for applications consistently across the data center fabric and the WAN is an important business enabler.

 
8. SDN Use Cases in the Enterprise
  * Alpha
  * Bravo
9. SDN Use Cases in Mobile Networks
  * Alpha
  * Bravo
10. The six characteristics of an SDN Network (Plane Separation, Simplified Forwarding Element, Centralized Control, Network Automation, Virtualization, and Openness)
  * Plane Separation: Control and management planes separated from data plane. Network control is directly programmable.
  * Simplified Forwarding Element: Packet switch simplification, no control logic, just forwarding function.
  * Centralized Control: Control/management plane logic move to a Controller. Network intelligence is (logically) centralized in an SDN controller(s) that maintains a global network view and the network appears to applications and policy engines as a single, logical switch. The controller is an external entity which may run a Network Operating System (NOS) that runs on a commodity server and facilitates abstractions for programming packet switch. The controller allows the execution of programs and software applications run on top of the NOS  while the NOS interacts with the underlying packet switches
  * Network Automation: Programmability and Agility: Programmatic configuration at user, network, switch, packet level which allows better management of the network; dynamic configuration and management to adjust/adapt network-wide traffic flow conforming the current needs. Security and resource optimization is based on automated SDN programs.
  * Virtualization.
  * Openness: Based on open standards and vendor-neutral. this simplifies network design as operation instructions are provided by SDN controllers and not multiple, vendor-specific devices and protocols. Control programs do not depend on proprietary software


11. SDN Devices (Controllers, Switches, Orchestration, API's)
  * Controllers: An SDN Controller in a software-defined network (SDN) contains the intelligence of the network. The controller is the logical/strategic control point in the SDN network, communicating with and relaying information to the switches ‘below’ (via southbound APIs) to provide networking instructions and the applications and business logic ‘above’ (via northbound APIs). 
  * Switches: An SDN switch is a software program or hardware device that forwards packets in a software-defined networking (SDN) environment. OpenFlow SDN switches are either based on the OpenFlow protocol or compatible with it. In a traditional network switch, packet forwarding (the data plane) and high-level routing (the control plane) occur on the same device. In software-defined networking, the data plane is decoupled from the control plane. The data plane is still implemented in the switch itself but the control plane is implemented in software and a separate SDN controller makes high-level routing decisions. The switch and controller communicate by means of the OpenFlow protocol.
  * Orchestration: Orchestration in a network context can be defined as the use of the automation to provide services using applications that drive the network. Software-defined networking (SDN) orchestration is the ability to program automated behaviours in a network to coordinate the required networking hardware and software elements to support applications and services.
  * API's: An API is an interface presented by an application/software (e.g. network operating system) that provides the capability to collect information from or make a change to an underlying set of resources. In SDN, there are two classes of API seeing great development and debate, Northbound Interfaces (NBI) and Southbound Interface (SDI).
   1. The southbound application program interfaces (APIs) are used to communicate between the SDN Controller and the switches and routers of the network. They can be open or proprietary. 
The most well-known southbound interface is OpenFlow, others include:

			   - NetConf using XML
			   - LISP
			   - Cisco OnePK
			   - Brocade OpenScript.
			   
   2. The northbound application program interfaces (APIs) are used to communicate between the SDN Controller and the services and applications running over the network. The northbound APIs can be used to facilitate innovation and enable efficient orchestration and automation of the network to align with the needs of different applications via SDN network programmability. One of the benefits of an API is the abstraction it provides to a querying system. This abstraction hides the underlying system from the querying system and frees it from such considerations as:

			   + the remote system’s query commands.
			   + how information is organized.
			   + the cli structures or restrictions in order to obtain information.

  
12. Overlay Networking Abstractions (NFV, VxLAN, etc.)
  * NFV: Network Functions Virtualisation aims to transform network architecture by evolving standard IT virtualisation technology to consolidate many network equipment types onto industry standard high volume servers, switches and storage, which could be located in Datacentres, Network Nodes and in the end user premises. It involves the implementation of network functions in software that can run on a range of industry standard server hardware, and that can be moved to, or instantiated in, various locations in the network as required, without the need for installation of new equipment.
  * VxLAN: VXLAN is a L2 in L3 tunneling mechanism that supports L2 learning and tenancy information.
  * STT
  * NVGRE
  * GENEVE

 
### DOMAIN 3: OPENFLOW® 25%
13. Identify at a concept/definition level the OpenFlow® Protocol operations and list the packet types and contents.

	The first resort should be the ONF OpenFlow specification documents, the various versions can be found [here] (), [here] (), [here] (), [here] (), [here] (), [here] (), [here] () and up to [2.0] (). [Flowgrammable] (http://flowgrammable.org/) is also a great site for a concise comparision of the different protocol version. The table below is gotten from the [Message Layer] (http://flowgrammable.org/sdn/openflow/message-layer/) page and the entire site is worth spending a couple of hours on.

  * TCP level secure channel/communication/session establishment between controller/switch: OpenFlow uses TCP as its transport protocol. Well known TCP ports for OpenFlow traffic are 6633 and 6653
  * Message Types: OpenFlow messages are used for communication between the controller and the switch for establishing the connection, sending the flows, polling the flow/port statistics, and notifying the controller etc. Every OpenFlow message begins with the same header structure. This fixed structure serves three roles that are independent of the version of OpenFlow being used. First, the version field indicates the version of OpenFlow which this message belongs. Second, the length field indicates where this message will end in the byte stream starting from the first byte of the header. Third, the xid, or transaction identifier, is a unique value used to match requests to responses. The type field which indicates what type of message is present and how to interpret the payload, is version dependent.
  * ![OpenFlow Messages] (https://github.com/driftavalli/ONF-Certified-Associate-Study-notes/blob/master/Snippet.png)

  

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
  * When a packet arrives at an OpenFlow switch, the header fields are compared to the table entries. If a match in the table entries is found, the packet is either forwarded to the specified port/ports or dropped. If a match isn’t found, the packet is sent to the controller. The controller informs the switch how the packet is to be processed and to create a new flow entry. 

### DOMAIN 4: SDN ARCHITECTURE AND ECOSYSTEM 25%
Understand and Identify SDN architectural components, standards bodies, controller design, API’s and applications.
  * Alpha
  * Bravo

1. SDN Layers
  * Alpha
  * Bravo
2. SDN Architecture compared to Traditional Network Architectures
  * Alpha
  * Bravo
3. Northbound API's
  * Alpha
  * Bravo
4. Southbound API's
  * Alpha
  * Bravo
5. East/West API's
  * Alpha
  * Bravo
6. Security and Availability
  * Alpha
  * Bravo
7. Packet and Optical Integration methods
  * Alpha
  * Bravo
8. Migration Strategies
  * Alpha
  * Bravo
9. Hybrid Mode Switches
  * HP Provision Switches
  * Brocade VDX

11. Organization in the SDN Ecosystem
  * Alpha
  * Bravo
12. Standards Bodies and Industry alliances
  * ONF (Open Networking Foundation)
  * ETSI (European Telecommunication Standards Institute)
  * IETF (Internet Engineering Task Force)
  * IEEE (Institute of Electrical and Electronic Engineers)
  * IMTC (International Multimedia Telecommunications Consortium)ITU (International Telecommunications Union)
  * 
  
13. Network Operators and Enterprises
  * Verizon
  * NTT
  * Deutsche Telekom
  * AT&T
  * Google
  * Orange
  * Vodafone

14. Network Equipment Manufacturers
  * HP (2920, 3500, 3800, 5400 ProCurve switches, )
  * Brocade (ADX, CER 2000, CES 2000, MLX)
  * Extreme Networks (Summit X670
  * Cisco
  * Juniper
  * BigSwitch Networks
  * Pica8
  * IBM RackSwitch G8264T
  * Infinera - DTN-X
  * A10 Networks – AX Series

15. Software vendors
  * Juniper (Contrail, OpenContrail, NorthStar WAN SDN Controller)
  * NEC (ProgrammableFlow Controller)
  * HP (HP VAN SDN Controller)
  * Cisco (Open SDN Controller, Application Policy Infrastructure Controller, APIC)
  * Brocade (Vyatta Controller)
  * B4N Controller
  * Ericsson SDN Controller
  * Extreme Networks OneController
  * IBM Programmable Network Controller
  * Inocybe Infrastructure Controller
  * Nuage Virtualized Services Controller (VSC)
  * Pica8 Integrated Open OVS Switch & Controller
  * Plexxi Control

  
16. Academic and Industry research institutions and labs
  * Open Networking La (ON.LAB)
  * Stanford Clean Slate Project
  * Open Networking Research Center (ONRC)
  * Electronics and Telecommunications Research Institute (ETRI)
  * International Computer Science Institute (ICSI)
  * Internet2
  * Centre of Excellence in Next Generation Networks (CENGN)
  * China Academy of Telecommunication Research, MIIT
  * University of New Hampshire InterOperability Laboratory (UNH-IOL)

17. Open Source Initiatives
  * Open vSwitch
  * OpenDaylight
  * OpenStack Foundation
  * OpenConfig
  * OpenCloud Connect
  * Open Compute Project
  * Open Container Project
  * Open Networking Summit
  * OPNFV
  * P4
  * Open Virtual Alliance
  * Multimedia and Mobile Communications Lab (MMLab)
  
18. Who is the ONF and what do they do?
  * Launched in 2011 by Deutsche Telekom, Facebook, Google, Microsoft, Verizon, and Yahoo!, ONF is a nonprofit organization dedicated to rethinking networking, and quickly and collaboratively bringing to market SDN standards and solutions. ONF is accelerating the delivery and commercialization of SDN and fostering a vibrant market of products, services, applications, customers, and users. The ONF is a user driven organization that is dedicated to accelerating the adoption of open Software-Defined Networking (SDN). 
 
19. Purpose
  * ONF develops open standards such as the OpenFlow® Standard and the OpenFlow® Configuration and Management Protocol Standard. The OpenFlow® Standard is the first and only vendor-neutral standard communications interface defined between the control and forwarding layers of an SDN architecture. ONF working groups also work on providing interoperable solution development on SDN concepts such as frameworks, architecture, and standards.
  
20. Structure
  * Alpha
  * Bravo
21. Technical Working Groups
  * Architecture and Framework.
  * Forwarding Abstraction.
  * Northbound Interfaces.
  * Discussion Groups.
  * Configuration and Management.
  * Market Education.
  * Optical Transport.
  * Wireless & Mobile.
  * Extensibility.
  * Migration.
  * Testing and Interoperability
  
22. Open Source Software Development
  * Alpha
  * Bravo
23. Activities and Initiatives
  * ONF-Certified SDN Professional (OCSP): A certification program will provide vendor-neutral SDN credentials to complement certifications in other technologies and programming languages. 
  * ONF OpenFlow Conformance Testing Program: Conformance tests performed at independent, accredited labs that verify networking hardware and software from various vendors to assure compliance with the OpenFlow specification.
  * Organizing PlugFest interoperability events, etc
 
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
  * Indigo is an open source project to support OpenFlow on a range of physical and virtual switch platforms.  The Indigo architecture (Indigo-2 architecture) is specified in the header files in the indigo module.
 
4. Linc
  * LINC is a pure OpenFlow software switch written in Erlang. It has the following features:
     - Support for OpenFlow Protocol 1.2, OpenFlow Protocol 1.3, and OpenFlow Protocol 1.4,
     - OpenFlow Capable Switch - ability to run multiple logical switches,
     - Support for OF-Config 1.1.1 management protocol,
     - Modular architecture, easily extensible.

5. OVS
  * Open vSwitch is a multilayer software switch licensed under the open source Apache 2 license. The aim is a production quality switch platform that supports standard management interfaces and opens the forwarding functions to programmatic extension and control. It currently supports:
     + Standard 802.1Q VLAN model with trunk and access ports
     + NIC bonding with or without LACP on upstream switch
     + NetFlow, sFlow(R), and mirroring for increased visibility
     + QoS (Quality of Service) configuration, plus policing
     + Geneve, GRE, GRE over IPSEC, VXLAN, and LISP tunneling
     + 802.1ag connectivity fault management
     + OpenFlow 1.0 plus numerous extensions
     + Transactional configuration database with C and Python bindings
     + High-performance forwarding using a Linux kernel module

6. CPqD/ONF Driver (aka "libFluid")
  * libfluid is a library bundle that provides the basic features to implement an OpenFlow controller. It is composed of two separate libraries:
     * libfluid_base: classes for creating an OpenFlow server that listens to connections and handles events
     * libfluid_msg: classes for easily building and parsing OpenFlow wire format messages
  
7. OpenFlow® Controllers
  * An OpenFlow Controller is a type of SDN Controller that uses the OpenFlow Protocol.  OpenFlow Controllers create a central control point to oversee a variety of OpenFlow-enabled network components. The OpenFlow protocol is designed to increase flexibility by eliminating proprietary protocols from hardware vendors. An SDN Controller relays information to the switches/routers ‘below’ (via southbound APIs) and the applications and business logic ‘above’ (via northbound APIs).
  
8. NOX
  * NOX is a Network Operating System that provides control and visibility into a network of OpenFlow switches. It supports concurrent applications written in Python and C++, and it includes a number of sample controller applications.

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
