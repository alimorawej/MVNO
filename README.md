# MVNO
Mobile Virtual Network Operator 

<figure>
 <img src="High Level Design/MVNO-overview.png" width="%65" height="%65">
 </figure>
 
## Introduction
<p>The MVNO concept is a very attractive option for such a “specialist”, aiming at drastically reducing the required resources (investment, headcount and roll-out time) and allowing the new entrant to focus on the really critical, market-side success factors. As there is no need for a spectrum license, a lengthy, complex and expensive radio network roll-out, or ongoing maintenance of the latter, market entry barriers are much lower than for a full mobile network operator (MNO). </p>

## Overview & description
<p>The principle of having a solution that combined all of the functionality required for an 3G/4G/LTE and IMS subscriber management and services platform that bundles the subscriber gateway services, and content delivery services into a single and completely virtual and represent the next generation of mobile network core platform.</p>
<p>The system architecture should have designed to meet the increased network capacities realized with 3G and 3G+ radio networks. The core networks solution should be providing broader and more intelligent subscriber services that operate on subscriber data and support the increase in demand to control content delivery providing the mobile operator with tools to monetize the content that flows through their radio network. </p>
<figure>
 <img src="High Level Design/MVNO-3G Core Network.png" width="%65" height="%65">
 <figcaption>Figure 1: 3G Core Network </figcaption>
 </figure>
 <br />
 
<p>The core network fulfills subscriber management functions defined in the 3GPP specifications in the role of mobility management (GGSN, SGSN, MME, SGW, PGW), policy and charging control, content and video optimization, and more with advanced features such as real-time analytics.
<p>Virtualized Mobile Core (VMC) solutions should support commercially available virtualization hypervisors (e.g., VMware, Linux KVM) and is designed to be deployed on Common Off The Shelf (COTS) hardware that enables mobile operators to quickly and cost-effectively increase the speed and performance of network.</p>
<p>This VMC solution should be support Dynamic Capacity Scaling. Operators able to configure Core KPIs (number of sessions or subscribers, CPU Load, throughput) in the system that will trigger the SGSN / MME or GGSN / SGW / PGW /VAS VNFs to add or remove Virtual Machines automatically in the operator’s data center. Also should be fully compliant with the Network Function Virtualization (NFV) architecture.</p>

## Simplified Network Management
<p>The network solution integrates seamlessly with operations, administration, and management (OA&M) layer to provide unified visibility and control across the entire networks. The Virtual Element Management System should allow for simplified, centralized provisioning and management of EPC functions and services for greater agility and flexibility. The VNF Manager should allow the operator to create, provisions, and instantiate a virtualized mobile core.</p>
<p>The software-defined core implements should support all the functions and protocols of GSM/GPRS and LTE core networks in software, and uses commodity hardware. </p>
<p>The software should be integrating the MSC / VLR / SGSN / GGSN / GMSC nodes from the GSM/GPRS core network. Also act as based on replacing the Base Station Subsystem with the software for GSM network such as BSC, NodeB and eNodeB with the Software.</p>

## 3G and 4G Core Gateway Services
<p>The system should provide SGW and PGW services that are part of the LTE as Evolved Packet Core (EPC) architecture as well as the GGSN service for 3G networks.</p>
<p>Operators able to configure the system as an SGW, PGW, or Service and Packet Gateway. The system architecture should be support both an SGW and PGW.</p>
<p>The system architecture should be support multiple VPN contexts enabling Operators to define multiple types of services as part of each VPN context. The system should be support the default context local, which is a global context. </p>

## Home Subscriber Server / Home Location Register Module

<p> The HSS/HLR is an affordable subscriber management solution suited for MVNO. The combined HSS/HLR is a clustered solution offering high reliability and redundancy. The HSS/HLR module should be exports any API for integration with any SIM management and CRM systems. It is capable of interconnecting with all the VLRs implemented in a GSM mobile network, with any MME from a conventional LTE network, or with the 3G core network server.</p>
<p>As it is also an AuC, the HSS/HLR authenticates subscribers as they try to connect to the GSM, UMTS, or the LTE networks, to make phone calls, send SMSs and access mobile data.</p>

## IP Multimedia Subsystem (IMS)

<p> The IMS core network is a scalable solution for operators who wish to start providing VoLTE multimedia services to their subscribers. The IMS is suited for small scale deployments and is easy to scale up as more users adopt the service.</p>
<p> IMS private and public should be identities per subscriber or SIP username, authentication, realm Domain and CSCF configuration (per profile) </p>
<p>High availability is required to be configured in a cluster of equal nodes Subscriber data is replicated across all nodes Requests can be distributed or balanced between nodes Detection of communication failures.</p>

<figure>
 <img src="High Level Design/MVNO_BlockDiagram_IMS.png" width="%65" height="%65">
 <figcaption>Figure 2: IMS Block Diagram</figcaption>
 </figure>
 <br />
