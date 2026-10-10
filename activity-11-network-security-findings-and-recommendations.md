# Activity 11: Network Security Findings and Recommendations

## 1. Introduction

Network security findings are observations made when reviewing a network's configuration, communication, and security controls. These findings can help identify weaknesses, assess potential risks, and recommend improvements.

Cybersecurity professionals must be able to explain technical findings clearly, understand their potential impact, and suggest practical actions to reduce risk.

The purpose of this activity is to consolidate the knowledge gained from previous activities and demonstrate how network security observations can be converted into useful recommendations.

## 2. Learning Objectives

The objectives of this activity are to:

* Identify common network security weaknesses.
* Understand the difference between a finding, a risk, and a recommendation.
* Assess the potential impact of network security issues.
* Prioritise security improvements according to risk.
* Produce clear and professional security recommendations.
* Understand the importance of privacy when documenting investigations.

## 3. Common Network Security Findings

### 3.1 Weak Wi-Fi Security

**Finding:** A wireless network may use outdated encryption or a weak password.

**Risk:** Unauthorised individuals may be able to gain network access or compromise the confidentiality of network communications.

**Recommendation:** Use WPA3 where supported, or WPA2-AES when WPA3 is unavailable. Set a strong, unique password and review router security settings.

### 3.2 Unnecessary Open Ports

**Finding:** A device may have listening ports associated with services that are not required.

**Risk:** Unnecessary services can increase the system's attack surface and may expose vulnerable applications.

**Recommendation:** Identify the service associated with each port, confirm whether it is required, and disable unnecessary services according to approved procedures.

### 3.3 Outdated Software and Firmware

**Finding:** A computer, router, or network device may be running software that no longer receives security updates or contains known vulnerabilities.

**Risk:** Attackers may exploit known weaknesses to gain unauthorised access, disrupt services, or compromise information.

**Recommendation:** Apply security updates regularly and replace unsupported devices where necessary.

### 3.4 Weak Passwords and Default Credentials

**Finding:** Users or administrators may use predictable passwords or retain default router credentials.

**Risk:** Attackers may guess or obtain credentials and gain unauthorised access to systems or network settings.

**Recommendation:** Use long, unique passwords, change default administrator credentials, and enable multifactor authentication where supported.

### 3.5 Inadequate Firewall Configuration

**Finding:** Firewall rules may permit unnecessary connections or fail to restrict traffic appropriately.

**Risk:** Unnecessary network access may increase exposure to unauthorised connections and attacks.

**Recommendation:** Review firewall rules, restrict access to what is required, and regularly check that rules remain appropriate.

### 3.6 Untrusted Public Wi-Fi

**Finding:** A user may connect to an unfamiliar or unverified public wireless hotspot.

**Risk:** The user may encounter fake hotspots, phishing pages, or attempts to intercept inadequately protected communications.

**Recommendation:** Verify hotspot names, use HTTPS, keep devices updated, and consider a reputable VPN when appropriate.

### 3.7 Unusual Network Connections

**Finding:** A device may communicate with an unfamiliar destination or use a connection that requires further investigation.

**Risk:** Depending on the context, the activity could indicate misconfiguration, an unapproved application, or potentially malicious communication.

**Recommendation:** Investigate the responsible process, destination, timing, and expected behaviour before deciding whether the connection represents a security issue.

An unfamiliar connection alone is not proof of malicious activity.

## 4. Understanding Risk Prioritisation

Security teams cannot always address every issue at once. They must prioritise findings according to factors such as likelihood, potential impact, exposure, and the effectiveness of existing security controls.

The following categories provide a simple example of prioritisation:

* **High:** A weakness that could result in serious harm or unauthorised access and requires prompt attention.
* **Medium:** A weakness that presents a meaningful risk but may have a more limited impact or require additional conditions to exploit.
* **Low:** A weakness with relatively limited potential impact that should still be addressed appropriately.

These categories are illustrative. A real organisation should use its own risk assessment method and consider the specific circumstances of each finding.

## 5. Example Network Security Findings Table

| Finding                           | Potential impact                                  | Example priority                     | Recommended action                      |
| --------------------------------- | ------------------------------------------------- | ------------------------------------ | --------------------------------------- |
| Outdated router security settings | Increased risk of unauthorised access             | High, depending on exposure          | Upgrade to supported security settings  |
| Weak Wi-Fi password               | Unauthorised network access                       | High, depending on circumstances     | Set a strong, unique password           |
| Unnecessary listening service     | Increased attack surface                          | Medium, depending on the service     | Review and disable if not required      |
| Missing software updates          | Exposure to known vulnerabilities                 | High, depending on the vulnerability | Apply appropriate security updates      |
| Unverified public Wi-Fi           | Exposure to deceptive hotspots                    | Medium, depending on usage           | Verify the network before connecting    |
| Unfamiliar network connection     | Possible unauthorised or unexpected communication | Requires investigation               | Identify the process and assess context |

The priorities in this table are examples, not confirmed ratings for a real network. Actual priorities depend on evidence, exposure, the system's importance, and the potential consequences.

## 6. Method for Investigating and Reporting Findings

A structured investigation helps ensure that findings are clear, accurate, and useful.

### Step 1: Identify the Observation

Record what was observed, such as an outdated security setting, an unexpected listening port, or a failed DNS lookup.

### Step 2: Collect Relevant Information

Use authorised tools and appropriate evidence to understand the issue. Avoid collecting unnecessary personal information.

### Step 3: Assess the Risk

Consider the likelihood of the issue being exploited and the potential impact on confidentiality, integrity, and availability.

### Step 4: Prioritise the Finding

Assign a priority using the organisation's risk assessment process. Explain the reasons for the rating.

### Step 5: Recommend an Action

Provide a practical recommendation that addresses the cause of the issue and reduces the associated risk.

### Step 6: Review the Outcome

Where appropriate, verify that the recommended change has been implemented and that the weakness has been reduced.

## 7. Relationship to the CIA Triad

Network security findings can affect the three principles of the CIA triad.

**Confidentiality:** Information should only be accessible to authorised people and systems. Weak Wi-Fi security or unauthorised access may threaten confidentiality.

**Integrity:** Information should remain accurate and protected against unauthorised changes. A compromised network device could allow an attacker to manipulate data or configuration.

**Availability:** Systems and information should remain accessible when needed. Denial-of-service attacks, network failures, or compromised infrastructure may affect availability.

Understanding these principles helps analysts explain why a finding matters and which security objectives could be affected.

## 8. Evidence and Privacy

No screenshots, raw network outputs, or packet captures are included in this report because they may expose private information such as IP addresses, gateway details, DNS servers, device names, and connection endpoints.

Publishing sensitive network information in a public GitHub repository may create unnecessary privacy and security risks.

The findings and recommendations in this report are presented as general learning examples based on the topics covered in the previous activities. They should not be interpreted as confirmed vulnerabilities discovered on a specific network.

Documenting the analysis in writing demonstrates an understanding of security assessment and responsible information handling without disclosing private network details.

## 9. Key Learning Outcomes

This activity reinforced the importance of identifying security weaknesses, assessing their potential impact, and recommending appropriate improvements.

The main learning outcomes are:

* Network security findings should be based on observations and evidence.
* Risk assessments should consider likelihood, impact, and exposure.
* Security recommendations should be specific and practical.
* Unfamiliar network activity requires investigation before conclusions are drawn.
* Security issues should be prioritised according to their actual risk.
* Privacy must be considered when storing and publishing investigation results.

## 10. Conclusion

This activity developed my understanding of how network security findings can be documented and translated into practical recommendations.

I learned how common weaknesses involving Wi-Fi security, passwords, firewall rules, software updates, listening ports, and network connections can create risks.

I also learned how to prioritise findings, relate risks to confidentiality, integrity, and availability, and recommend improvements based on the available evidence.

These skills are important for cybersecurity professionals because effective security work involves not only identifying problems but also explaining their impact and recommending appropriate solutions.

This activity provides a foundation for the final review of my Network Security Fundamentals project.
