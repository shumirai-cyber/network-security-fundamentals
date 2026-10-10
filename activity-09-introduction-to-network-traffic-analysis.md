# Activity 9: Introduction to Network Traffic Analysis

## 1. Introduction

Network traffic analysis is the process of examining data travelling across a computer network to understand communication between devices, identify unusual activity, and investigate potential security problems.

Cybersecurity professionals use network traffic analysis to monitor network performance, investigate suspicious connections, detect possible attacks, and support incident response.

The purpose of this activity is to understand how network traffic can be analysed, the tools used for analysis, and the importance of protecting sensitive network information.

## 2. Learning Objectives

The objectives of this activity are to:

* Understand what network traffic analysis is.
* Identify the difference between incoming and outgoing network traffic.
* Learn about network packets and protocols.
* Understand how traffic analysis can support cybersecurity investigations.
* Identify tools used to analyse network traffic.
* Recognise suspicious network activity.
* Understand privacy and ethical considerations when analysing network traffic.

## 3. What Is Network Traffic?

Network traffic is the data transmitted between devices over a network. This communication may take place across a local network, a wireless connection, or the internet.

Examples include:

* A web browser requesting a webpage from a web server.
* A computer connecting to a DNS server to resolve a domain name.
* An email application communicating with a mail server.
* A device downloading a software update.
* A computer connecting to a remote service.

Network traffic can be examined to understand which systems are communicating, which protocols are being used, and whether communication patterns appear normal or suspicious.

## 4. Network Packets

Data sent across computer networks is commonly divided into smaller units called packets.

A packet may contain information such as source and destination addresses, protocol information, and a portion of the transmitted data. The precise fields depend on the network protocol being used.

Analysing packets can help a security analyst understand how devices communicate and investigate unexpected connections.

However, packet information can also contain sensitive details. Captured traffic may expose private information if it is not properly protected, so packet captures should be handled carefully.

## 5. Incoming and Outgoing Traffic

### Incoming Traffic

Incoming traffic is data received by a device from another device or network.

Examples include receiving a webpage response, downloading a file, or receiving data from an online service.

Unexpected incoming connections may deserve investigation, especially when they involve exposed services or unauthorised access attempts.

### Outgoing Traffic

Outgoing traffic is data sent from a device to another destination.

Examples include browsing websites, sending emails, and connecting to cloud services.

Unusual outgoing traffic may indicate a misconfigured application, an unauthorised connection, or potentially malicious software communicating with an external system.

Neither incoming nor outgoing traffic is automatically malicious. The context, destination, application, and expected behaviour must be considered.

## 6. Common Network Protocols

The following protocols commonly appear during network traffic analysis:

* **TCP:** Provides reliable, ordered data delivery between applications.
* **UDP:** Sends datagrams without guaranteeing delivery or ordering.
* **DNS:** Translates domain names into information used to locate internet services.
* **HTTP:** Transfers web content without providing transport encryption by itself.
* **HTTPS:** Protects web communication using TLS encryption.
* **DHCP:** Helps devices obtain IP configuration automatically.
* **ICMP:** Supports network diagnostics and error reporting, including the use of tools such as ping.

Understanding these protocols helps analysts recognise normal communication and investigate activity that does not match expected patterns.

## 7. Network Traffic Analysis Tools

### 7.1 Wireshark

Wireshark is a network protocol analyser that allows users to capture and inspect packets from network interfaces or analyse previously saved capture files.

It can help analysts investigate protocols, communication between devices, and unusual traffic patterns.

### 7.2 tcpdump

tcpdump is a command-line packet analysis tool commonly used on Linux and other supported systems. It can capture and display network packets according to selected filters.

### 7.3 Windows Networking Tools

Windows includes built-in tools such as `netstat`, `ping`, `tracert`, and `nslookup`.

These tools provide useful information about connections, network reachability, routing paths, and DNS resolution. They do not replace a full packet analyser, but they can support initial investigations.

## 8. How Traffic Analysis Supports Cybersecurity

Network traffic analysis can support several important security tasks.

### Detecting Suspicious Connections

Analysts can investigate connections to unexpected destinations, unusual ports, or services that should not be communicating.

### Identifying Potential Malware Activity

Some forms of malware communicate with external systems. Unusual connection patterns may provide clues that warrant further investigation, although suspicious traffic alone does not prove that a device is infected.

### Investigating Denial-of-Service Activity

A large or unusual volume of traffic directed at a service may indicate a possible denial-of-service incident. Analysts must distinguish malicious activity from legitimate increases in demand.

### Supporting Incident Response

Traffic analysis can help establish a timeline, identify affected systems, understand communication patterns, and support decisions about containment and recovery.

## 9. Practical Investigation

The practical objective of this activity is to understand how network communication can be observed and interpreted using appropriate tools.

A basic investigation can follow these steps:

1. Identify the device or network interface being investigated.
2. Establish the purpose and authorised scope of the investigation.
3. Use an appropriate tool to examine available connection or traffic information.
4. Identify relevant protocols and connection states.
5. Look for unusual destinations, unexpected services, or patterns that require further investigation.
6. Compare observations with expected system behaviour.
7. Record findings and recommend appropriate follow-up actions.

A packet analyser such as Wireshark can be used to inspect traffic in a controlled environment. For beginner investigations, a previously saved sample capture or authorised lab environment can reduce the risk of exposing personal information.

### Interpreting Findings

An unusual connection does not automatically indicate an attack. Security analysts must consider the application involved, the destination, the time of the connection, and whether the activity is expected.

Reliable conclusions require sufficient evidence and appropriate context.

## 10. Security Recommendations

The following recommendations support safer network traffic monitoring:

* Use approved tools and investigate only networks for which permission has been granted.
* Keep network monitoring tools updated.
* Protect packet captures and investigation notes.
* Avoid publishing raw traffic captures, private IP addresses, public IP addresses, device names, or other sensitive information in a public repository.
* Investigate unusual connections before drawing conclusions.
* Use secure protocols and appropriate network controls.
* Restrict access to collected network data.
* Retain investigation evidence only as long as necessary and in accordance with applicable policies.

## 11. Evidence and Privacy

No screenshots, packet captures, or raw network outputs are included in this report because they may reveal private information, including IP addresses, device details, DNS information, connection endpoints, and other network activity.

Network traffic can contain sensitive information belonging to the user or other people. Publishing raw traffic data could expose details that are not appropriate for a public cybersecurity portfolio.

The investigation process and learning outcomes are documented in writing instead. This demonstrates an understanding of network traffic analysis while respecting privacy and responsible information handling.

## 12. Conclusion

This activity developed my understanding of network traffic analysis and its role in cybersecurity.

I learned about network packets, incoming and outgoing traffic, common network protocols, and tools such as Wireshark, tcpdump, and Windows networking utilities.

I also learned that network traffic analysis can help identify suspicious activity and support security investigations, but findings must be interpreted carefully and supported by evidence.

Finally, this activity reinforced the importance of authorised investigations, protecting captured data, and avoiding the publication of sensitive network information.

These skills provide a foundation for further learning in network monitoring, threat detection, and incident response.
