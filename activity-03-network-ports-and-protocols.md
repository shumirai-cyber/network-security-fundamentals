# Activity 3: Network Ports and Protocols

## 1. Objective

The objective of this activity was to understand network ports, communication protocols, and how Windows can be used to inspect network connections and listening endpoints.

## 2. What Are Network Ports?

A network port is a numbered communication endpoint used to direct network traffic to the appropriate application or service.

Ports help a computer handle different types of network communication. For example, a computer can use one service for web browsing and another for remote administration.

## 3. What Are Network Protocols?

Network protocols are rules that allow devices to communicate across networks.

Two important transport protocols are:

* **TCP (Transmission Control Protocol):** Provides reliable, ordered delivery of data.
* **UDP (User Datagram Protocol):** Sends data without guaranteeing delivery or order, making it useful for applications that prioritise speed or low overhead.

Different applications use different protocols and ports depending on their purpose.

## 4. Common Network Ports

| Port | Service | Typical purpose                    |
| ---- | ------- | ---------------------------------- |
| 22   | SSH     | Secure remote administration       |
| 25   | SMTP    | Sending email between mail servers |
| 53   | DNS     | Resolving domain names             |
| 80   | HTTP    | Unencrypted web traffic            |
| 443  | HTTPS   | Encrypted web traffic using TLS    |
| 3389 | RDP     | Remote Desktop access on Windows   |

These are common default ports. Actual configurations can vary depending on the service and environment.

## 5. Practical Exercise: Windows Netstat

I used the Windows Command Prompt to run the following command:

`netstat -ano`

The command completed successfully and displayed network connection information.

I observed entries containing local addresses, foreign addresses, connection states, and process IDs. The results helped me understand how Windows reports network connections and listening endpoints.

The command options have the following meanings:

* `-a`: Displays active connections and listening TCP and UDP ports.
* `-n`: Displays addresses and port numbers numerically.
* `-o`: Displays the process ID associated with each connection.

For TCP connections, the `LISTENING` state indicates that a service is waiting for incoming connections, while `ESTABLISHED` indicates an active TCP connection.

## 6. Cybersecurity Importance

Understanding network ports and protocols is important because exposed or unnecessary services can increase a system's attack surface.

Security professionals can investigate listening ports, identify the applications associated with them, and determine whether network access is appropriately restricted.

A listening port is not automatically a security problem. Its purpose, configuration, exposure, and business requirements must be considered before deciding whether action is needed.

## 7. Privacy Considerations

The command output contained network information that I did not want to publish in a public repository.

I chose to document the command, its purpose, and my observations in writing instead of uploading a screenshot containing potentially sensitive details.

This demonstrates the importance of protecting technical information when preparing cybersecurity portfolio evidence.

## 8. Key Learning Outcomes

Through this activity, I learned that:

* Network ports help direct traffic to the appropriate services.
* TCP and UDP provide different approaches to transporting data.
* Common services often use well-known default port numbers.
* The Windows `netstat -ano` command can display connections, listening endpoints, and process IDs.
* Listening ports should be investigated in context rather than automatically treated as threats.
* Network investigation evidence should be handled carefully to protect privacy.

## 9. Conclusion

This activity gave me practical experience using a built-in Windows networking command. I learned how to inspect network connection information and why ports, protocols, and listening services matter in network security.

**Activity status:** Practical exercise completed and documented. No screenshot published because the command output contained private network information.
