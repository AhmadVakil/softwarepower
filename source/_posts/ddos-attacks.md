---
title: DDoS attacks
date: 2016-03-24T02:38:43.606Z
updated: 2016-03-24T02:38:00.000Z
category:
  - Security & Hacking
comments: true
---
**Denial-of-service (DoS) and distributed denial-of-service (DDoS) attacks**

{% youtube ilhGh9CEIwM %}

A denial-of-service attack overwhelms a system’s resources so that it cannot respond to service requests. A DDoS attack is also an attack on system’s resources, but it is launched from a large number of other host machines that are infected by malicious software controlled by the attacker.



Unlike attacks that are designed to enable the attacker to gain or increase access, denial-of-service doesn’t provide direct benefits for attackers. For some of them, it’s enough to have the satisfaction of service denial. However, if the attacked resource belongs to a business competitor, then the benefit to the attacker may be real enough. Another purpose of a DoS attack can be to take a system offline so that a different kind of attack can be launched. One common example is session hijacking, which I’ll describe later.



There are different types of DoS and DDoS attacks; the most common are TCP SYN flood attack, teardrop attack, smurf attack, ping-of-death attack and botnets.



TCP SYN flood attack

In this attack, an attacker exploits the use of the buffer space during a Transmission Control Protocol (TCP) session initialization handshake. The attacker’s device floods the target system’s small in-process queue with connection requests, but it does not respond when the target system replies to those requests. This causes the target system to time out while waiting for the response from the attacker’s device, which makes the system crash or become unusable when the connection queue fills up.



There are a few countermeasures to a TCP SYN flood attack:



Place servers behind a firewall configured to stop inbound SYN packets.

Increase the size of the connection queue and decrease the timeout on open connections.

Teardrop attack

This attack causes the length and fragmentation offset fields in sequential Internet Protocol (IP) packets to overlap one another on the attacked host; the attacked system attempts to reconstruct packets during the process but fails. The target system then becomes confused and crashes.



If users don’t have patches to protect against this DoS attack, disable SMBv2 and block ports 139 and 445.



Smurf attack

This attack involves using IP spoofing and the ICMP to saturate a target network with traffic. This attack method uses ICMP echo requests targeted at broadcast IP addresses. These ICMP requests originate from a spoofed “victim” address. For instance, if the intended victim address is 10.0.0.10, the attacker would spoof an ICMP echo request from 10.0.0.10 to the broadcast address 10.255.255.255. This request would go to all IPs in the range, with all the responses going back to 10.0.0.10, overwhelming the network. This process is repeatable, and can be automated to generate huge amounts of network congestion.



To protect your devices from this attack, you need to disable IP-directed broadcasts at the routers. This will prevent the ICMP echo broadcast request at the network devices. Another option would be to configure the end systems to keep them from responding to ICMP packets from broadcast addresses.



Ping of death attack

This type of attack uses IP packets to ‘ping a target system with an IP size over the maximum of 65,535 bytes. IP packets of this size are not allowed, so attacker fragments the IP packet. Once the target system reassembles the packet, it can experience buffer overflows and other crashes.



Ping of death attacks can be blocked by using a firewall that will check fragmented IP packets for maximum size.



Botnets

Botnets are the millions of systems infected with malware under hacker control in order to carry out DDoS attacks. These bots or zombie systems are used to carry out attacks against the target systems, often overwhelming the target system’s bandwidth and processing capabilities. These DDoS attacks are difficult to trace because botnets are located in differing geographic locations.



Botnets can be mitigated by:



RFC3704 filtering, which will deny traffic from spoofed addresses and help ensure that traffic is traceable to its correct source network. For example, RFC3704 filtering will drop packets from bogon list addresses.

Black hole filtering, which drops undesirable traffic before it enters a protected network. When a DDoS attack is detected, the BGP (Border Gateway Protocol) host should send routing updates to ISP routers so that they route all traffic heading to victim servers to a null0 interface at the next hop.

Resource: blog.netwrix.com
