# Activity 2: IP Addresses and Subnet Basics

## 1. Objective

The objective of this activity is to understand IP addresses, subnet masks, and subnets, and how they help devices communicate across networks.

## 2. What Is an IP Address?

An IP (Internet Protocol) address is a logical address used to identify a network interface so that data can be sent to the correct destination.

There are two main versions of IP addresses:

* **IPv4:** Uses four numbers separated by dots, for example, `192.168.1.25`.
* **IPv6:** Uses hexadecimal characters separated by colons and supports a much larger address space than IPv4.

IP addresses help devices communicate with other devices on the same network or across different networks.

## 3. What Is a Subnet Mask?

A subnet mask is used with an IPv4 address to identify the network portion and the host portion of the address.

For example, `255.255.255.0` is a common subnet mask, equivalent to a `/24` prefix. In this case, the first 24 bits represent the network portion, while the remaining 8 bits represent the host portion.

Subnet masks help devices determine whether a destination is on the local network or whether traffic needs to be sent through a router.

## 4. What Is a Subnet?

A subnet is a logical section of a larger IP network. Subnetting allows networks to be divided into smaller sections to improve organisation and manage IP addresses more efficiently.

In cybersecurity, network segmentation can also help separate systems and restrict unnecessary communication between different parts of a network.

## 5. Learning Activity

In Activity 1, I used the Windows Command Prompt and the `ipconfig` command to examine my computer's network configuration.

This helped me understand that Windows can display network information, including IPv4 addresses, subnet masks, and default gateways.

I am using the existing screenshot from Activity 1 as supporting evidence rather than uploading a duplicate.

**Evidence reference:** `evidence/activity-01-ipconfig.png`

## 6. Security and Privacy Considerations

Network configuration information can reveal details about a device and its local network. Before publishing screenshots in a public portfolio, I should check for sensitive or identifying information and redact it where appropriate.

Private IP addresses are generally not directly reachable from the public internet, but they can still reveal details about an internal network.

## 7. Key Learning Outcomes

Through this activity, I learned that:

* IP addresses identify network interfaces for communication.
* IPv4 and IPv6 are different versions of Internet Protocol addressing.
* Subnet masks help distinguish the network portion from the host portion of an IPv4 address.
* Subnets divide larger networks into smaller logical sections.
* Understanding IP addressing is important for network troubleshooting and cybersecurity.

## 8. Conclusion

Understanding IP addresses, subnet masks, and subnets provides a foundation for learning how networks operate. These concepts are useful when investigating network configurations, troubleshooting connectivity problems, and understanding how networks can be organised securely.

**Activity status:** Documentation completed; existing screenshot referenced as supporting evidence.
