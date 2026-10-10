# Activity 5: Routers, Switches and Network Devices

## Objective

To understand the roles of routers, switches, wireless access points and Ethernet cables, and investigate how data travels across a network.

## 1. Routers

A router connects different networks and forwards data between them using IP addresses. For example, a home router connects devices on a local network to the internet.

Routers help data reach its intended destination and may provide additional features such as firewall protection and wireless connectivity.

## 2. Switches

A network switch connects devices within a local area network (LAN), such as computers, printers and servers in an office.

Switches commonly use MAC addresses to forward Ethernet frames towards the appropriate devices.

## 3. Wireless Access Points

A wireless access point allows devices to connect to a network using Wi-Fi. It can be built into a home router or installed separately in offices and larger networks.

Wireless access points should be secured with strong passwords and modern Wi-Fi security settings to reduce the risk of unauthorised access.

## 4. Ethernet Cables

Ethernet cables provide wired connections between compatible network devices. Wired connections can offer reliable communication and avoid wireless-specific security risks.

However, wired networks still need appropriate security controls to prevent unauthorised access.

## 5. Practical Activity: Traceroute Investigation

I used Windows Command Prompt to run the following command:

`tracert google.com`

The command displayed IP addresses, numerical hop information and some asterisks.

### My observations

* **IP addresses:** These represented network interfaces that responded along the route towards the destination.
* **Numerical information:** The output included hop numbers and response times, usually measured in milliseconds.
* **Asterisks (*):** These indicated that some probes did not receive a response before the timeout.

Some network devices do not respond to traceroute probes. Therefore, asterisks do not necessarily indicate a network fault.

### What I learned

The `tracert` command is useful for investigating the route towards a destination and identifying where responses may be delayed or unavailable. However, it does not necessarily identify every device along the route.

## 6. Network Security Considerations

* Routers should use strong administrator passwords and updated firmware.
* Unnecessary remote administration services should be disabled.
* Network equipment should be protected from unauthorised physical access.
* Wireless access points should use strong Wi-Fi passwords and modern encryption.
* Network devices should be configured to allow only authorised connections where appropriate.
* Network diagnostic information should be reviewed before being shared publicly.

## 7. Key Learning Outcomes

After completing this activity, I understand that:

* Routers connect different networks and forward IP traffic.
* Switches connect devices within a LAN and commonly forward Ethernet frames using MAC addresses.
* Wireless access points provide Wi-Fi connectivity.
* Ethernet cables provide wired network connections.
* The `tracert` command helps investigate the route towards a destination.
* Asterisks in traceroute output can indicate unanswered probes rather than a network failure.
* Protecting network information is an important part of cybersecurity.

## 8. Evidence and Privacy

I completed the practical investigation using Windows Command Prompt. However, I have not uploaded screenshots or raw command output as evidence because the results contain multiple IP addresses and other network information that could reveal private details about my network.

To protect my privacy and demonstrate responsible cybersecurity practices, I have documented the command used, my observations and my learning outcomes in this written report instead of publishing potentially sensitive information.

## Conclusion

This activity helped me understand the roles of common network devices and how they support communication between computers and networks. I used `tracert google.com` to investigate a network route and learned how to interpret IP addresses, hop information, response times and unanswered probes.

I also learned that network security involves protecting both network equipment and the information produced during technical investigations.
