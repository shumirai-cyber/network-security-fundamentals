# Activity 4: DNS, DHCP and How Devices Connect

## Objective

To understand how DNS and DHCP help devices connect to networks and access websites.

## 1. What Is DNS?

DNS stands for Domain Name System. It translates human-readable domain names, such as `google.com`, into IP addresses that computers use to communicate with servers.

## 2. What Is DHCP?

DHCP stands for Dynamic Host Configuration Protocol. It automatically assigns network configuration settings to devices. These settings can include an IP address, subnet mask, default gateway and DNS server.

## 3. How Devices Connect

When a device joins a network, DHCP may provide its network settings automatically. When the user visits a website, DNS can resolve the website's domain name to an IP address. The device can then use that address to communicate with the website's server.

## 4. Practical Activity: DNS Lookup

I used Windows Command Prompt to run:

`nslookup google.com`

The command returned a DNS server address and multiple IP addresses for `google.com`. The results included both IPv4 and IPv6 addresses.

The DNS server was displayed as `Unknown`. This does not necessarily indicate a problem; the server's name may not be available through reverse DNS lookup.

## 5. Security and Privacy Considerations

* DNS helps devices locate online services.
* Incorrect or malicious DNS responses can redirect users to unwanted or fraudulent destinations.
* Attackers may use techniques such as DNS spoofing to interfere with name resolution.
* DHCP should be appropriately secured on networks to reduce the risk of unauthorised devices or rogue DHCP servers providing incorrect settings.
* Network command output may contain private information, so it should be reviewed before being shared publicly.

## 6. Key Learning Outcomes

* DNS translates domain names into IP addresses.
* DHCP automatically supplies network configuration settings.
* DNS lookups can return IPv4 and IPv6 addresses.
* A DNS server displayed as `Unknown` does not necessarily mean DNS has failed.
* DNS and DHCP are important parts of everyday network communication.

## Conclusion

This activity helped me understand how DNS and DHCP support network connectivity. I also used `nslookup` to investigate how a domain name is resolved into IP addresses and learned about related network security and privacy considerations.
