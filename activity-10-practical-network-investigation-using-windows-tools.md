# Activity 10: Practical Network Investigation Using Windows Tools

## 1. Introduction

Windows provides several built-in networking tools that help users and cybersecurity professionals investigate network connectivity, identify connection problems, and understand how devices communicate.

These tools can provide information about IP configuration, DNS resolution, network routes, active connections, and network reachability.

The purpose of this activity is to understand how Windows networking tools can support basic network investigations and how their results can be interpreted responsibly.

## 2. Learning Objectives

The objectives of this activity are to:

* Identify common Windows networking tools.
* Understand how to investigate network connectivity.
* Examine DNS resolution and network routing.
* Understand active network connections and listening ports.
* Interpret common command-line results.
* Recognise the limitations of basic network investigations.
* Protect sensitive network information when documenting findings.

## 3. Windows Networking Tools

### 3.1 ipconfig

The `ipconfig` command displays TCP/IP configuration information for network adapters.

It can help identify whether a device has an IP address, default gateway, and DNS server configuration.

Example command:

```cmd
ipconfig
```

The `ipconfig /all` command provides more detailed configuration information, including adapter details and additional network settings.

**Security relevance:** This information helps troubleshoot connectivity problems and understand how a device is configured on a network. However, the output may reveal private network details and should not be published without careful review.

### 3.2 ping

The `ping` command tests whether a destination responds to ICMP echo requests.

Example command:

```cmd
ping example.com
```

Successful replies can indicate that the destination is reachable through the tested path. However, some devices and networks block ICMP traffic, so a failed ping does not necessarily mean that a service is unavailable.

**Security relevance:** Ping can help identify basic connectivity problems, but it does not prove that a system is secure.

### 3.3 nslookup

The `nslookup` command helps investigate DNS resolution by querying DNS servers.

Example command:

```cmd
nslookup example.com
```

It can display the DNS server used for the query and the address records returned for a domain.

**Security relevance:** DNS investigation can help identify name-resolution problems and understand how domain names are resolved. Unexpected results may require further investigation, but they do not automatically indicate malicious activity.

### 3.4 tracert

The `tracert` command investigates the route taken by packets towards a destination.

Example command:

```cmd
tracert example.com
```

The output lists routing hops and the response times observed for each hop. An asterisk indicates that a probe did not receive a response within the relevant timeout period.

**Security relevance:** Traceroute can help investigate routing problems. Missing responses do not necessarily indicate an attack or network failure because routers may limit or block diagnostic responses.

### 3.5 netstat

The `netstat` command displays information about network connections and listening ports.

Example command:

```cmd
netstat -ano
```

Common options include:

* `-a`: Displays active connections and listening ports.
* `-n`: Displays addresses and port numbers numerically.
* `-o`: Displays the process identifier (PID) associated with each connection when available.

Common connection states include:

* **LISTENING:** A service is waiting for incoming connections on a TCP port.
* **ESTABLISHED:** A TCP connection has been established.
* **TIME_WAIT:** A connection is waiting for a period before its associated resources are fully released.

**Security relevance:** This tool can help identify unexpected listening ports and review active connections. A listening port or unfamiliar connection is not automatically malicious; further investigation is needed to understand the process and its purpose.

## 4. Practical Network Investigation

A basic network investigation can use several Windows tools to build an overview of a computer's network configuration and connectivity.

### Step 1: Review Network Configuration

Use `ipconfig` to understand how the computer receives its network configuration.

The information may include IPv4 or IPv6 addresses, a default gateway, and DNS server details.

### Step 2: Investigate DNS Resolution

Use `nslookup` with a domain name to understand how DNS translates that name into network addresses.

Review the returned results and note that one domain may resolve to multiple addresses.

### Step 3: Examine the Network Route

Use `tracert` with a domain name to observe the route towards the destination.

Consider the number of hops, response times, and any probes that time out. A timeout should be interpreted cautiously because intermediate routers may not respond to every diagnostic request.

### Step 4: Review Network Connections

Use `netstat -ano` to examine active connections and listening ports.

Consider whether the connection states and services appear consistent with normal computer use. Avoid assuming that a connection is malicious based only on its address or port.

### Step 5: Interpret the Results

Compare the information from the different tools to develop an understanding of the device's network behaviour.

For example, DNS resolution may work even when a particular service is unavailable. Similarly, a successful route investigation does not guarantee that an application or destination service is functioning correctly.

A reliable investigation considers multiple observations rather than relying on a single command.

## 5. Key Findings and Learning Outcomes

The investigation demonstrates that Windows includes useful tools for basic network troubleshooting and security awareness.

The main learning outcomes are:

* `ipconfig` helps review network configuration.
* `ping` tests basic reachability using ICMP.
* `nslookup` investigates DNS resolution.
* `tracert` provides information about routing paths.
* `netstat` helps examine active connections and listening ports.

These tools provide different types of information. Using them together can help develop a clearer understanding of network behaviour.

However, built-in Windows tools do not provide a complete security assessment. More advanced investigations may require approved monitoring tools, event logs, endpoint security software, or packet analysis.

## 6. Security Recommendations

Based on this activity, the following recommendations are appropriate:

1. Review network configuration when investigating connectivity problems.
2. Investigate unexpected listening ports and connections using approved methods.
3. Keep Windows and installed applications updated.
4. Use a firewall to control network communication according to appropriate security policies.
5. Avoid treating a single unusual result as proof of an attack.
6. Record findings clearly and distinguish observations from assumptions.
7. Only investigate systems and networks for which permission has been granted.
8. Protect command output that contains IP addresses, device names, DNS details, or connection endpoints.

## 7. Limitations of the Investigation

Basic command-line tools provide useful information, but they have limitations.

They may not explain why a particular connection exists, identify every application responsible for network activity, or prove that a system is free from malware.

Some network devices also block diagnostic traffic, limit responses, or use configurations that make results difficult to interpret.

Further investigation may be necessary before drawing conclusions about a suspected security issue.

## 8. Evidence and Privacy

No screenshots or raw command outputs are included in this report because they may contain private information, including IP addresses, gateway addresses, DNS servers, device details, and network connection endpoints.

Publishing this information in a public GitHub repository could unnecessarily expose personal or network configuration details.

The investigation methods and learning outcomes are therefore documented in writing instead. This approach demonstrates knowledge of Windows network investigation while respecting privacy and responsible information handling.

## 9. Conclusion

This activity developed my understanding of how Windows networking tools can support basic network investigations.

I learned how to use `ipconfig`, `ping`, `nslookup`, `tracert`, and `netstat` to examine network configuration, connectivity, DNS resolution, routing, and active connections.

I also learned the importance of interpreting results carefully, recognising the limitations of individual tools, and protecting sensitive network information.

These skills provide a foundation for further work in network troubleshooting, cybersecurity monitoring, and incident investigation.
