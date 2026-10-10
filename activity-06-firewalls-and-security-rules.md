# Activity 6: Firewalls and Network Security Rules

## Objective

To understand how firewalls protect computers and networks, learn about inbound and outbound traffic, and investigate the firewall status on my Windows computer.

## 1. What Is a Firewall?

A firewall is a security control that monitors and filters network traffic according to defined rules. It helps protect computers and networks by allowing legitimate traffic and restricting unwanted or unauthorised connections.

Firewalls can be implemented in software, hardware or a combination of both.

## 2. Inbound and Outbound Traffic

### Inbound traffic

Inbound traffic is network traffic attempting to enter a computer or network. Firewall rules can restrict incoming connections that are not permitted.

### Outbound traffic

Outbound traffic is network traffic leaving a computer or network. Firewall rules can also control outgoing connections where appropriate.

## 3. Firewall Rules

Firewall rules define which network traffic is allowed or blocked. Rules may consider factors such as:

* Inbound or outbound direction
* Network protocol, such as TCP or UDP
* Port number
* Application or service
* Network profile and other connection conditions

Appropriate firewall rules help reduce unnecessary exposure to network threats.

## 4. Windows Defender Firewall

Windows Defender Firewall is a built-in Windows security feature that helps filter network traffic.

Windows provides different network profiles, including:

* **Domain network:** Used for computers connected to an organisation's domain network.
* **Private network:** Intended for trusted networks, such as a trusted home network.
* **Public network:** Intended for less-trusted networks, such as public Wi-Fi.

The appropriate profile depends on the network and its trust level.

## 5. Practical Activity: Checking Firewall Status

I used the Windows Security application to investigate the firewall status.

### Steps completed

1. Opened Windows Security.
2. Selected Firewall & network protection.
3. Checked the displayed firewall status.

### Findings

The firewall was reported as turned on.

This indicates that Windows Firewall was enabled for the network profile I checked. An enabled firewall helps filter network traffic according to its configured rules.

I did not change any firewall settings because the purpose of this activity was to investigate the existing configuration safely.

## 6. Security Recommendations

* Keep Windows and security updates up to date.
* Keep the firewall enabled unless an authorised administrator has a specific reason to change its configuration.
* Avoid allowing applications through the firewall unless they are trusted and the access is necessary.
* Review firewall rules periodically.
* Use an appropriate network profile for the network being connected to.
* Use strong passwords and other security controls alongside the firewall.
* Investigate unexpected security warnings rather than ignoring them.

## 7. Key Learning Outcomes

After completing this activity, I understand that:

* Firewalls filter network traffic according to rules.
* Inbound traffic enters a device or network, while outbound traffic leaves it.
* Firewall rules can use protocols, ports, applications and other conditions.
* Windows Defender Firewall provides built-in network protection.
* Windows has Domain, Private and Public network profiles.
* An enabled firewall is important, but it does not guarantee complete security.
* Checking security settings without changing them is a useful first step in a safe investigation.

## 8. Evidence and Privacy

I completed the practical investigation using Windows Security. However, I have not uploaded screenshots or raw command output as evidence because security configuration details and network information may reveal private information about my computer or network.

To protect my privacy and demonstrate responsible cybersecurity practices, I have documented the investigation steps, findings and learning outcomes in this written report instead of publishing potentially sensitive information.

## Conclusion

This activity helped me understand how firewalls filter network traffic and how inbound and outbound connections differ. I used Windows Security to check my firewall status and confirmed that the firewall was turned on.

I also learned that firewalls are an important part of a wider security strategy and that protecting privacy during technical investigations is a responsible cybersecurity practice.
