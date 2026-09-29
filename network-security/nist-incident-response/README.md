# Applying the NIST CSF – ICMP Flood Incident

## Overview

This project demonstrates the application of the NIST Cybersecurity Framework (NIST CSF) to analyze and respond to a network security incident.

The scenario involves a Denial-of-Service (DoS) attack caused by an ICMP flood, which disrupted the organization's network services and prevented normal internal traffic from accessing network resources.

The incident was analyzed using the five core functions of the NIST CSF:

- Identify
- Protect
- Detect
- Respond
- Recover

This exercise was completed as part of the Google Cybersecurity Certificate.

---

## Scenario

A multimedia company experienced a network outage caused by an ICMP flood attack.

A malicious actor sent a large volume of ICMP packets through a misconfigured firewall, overwhelming the organization's network and preventing normal network traffic from accessing internal resources.

The incident response team:

- Blocked incoming ICMP packets
- Took non-critical network services offline
- Restored critical network services
- Investigated the source and characteristics of the attack

The security team subsequently implemented additional security measures to reduce the risk of similar incidents.

---

## Investigation

The incident was analyzed by examining the affected network services, the firewall configuration, the characteristics of the ICMP traffic, and the organization's response.

The investigation identified:

- An ICMP flood causing a Denial-of-Service condition
- A misconfigured firewall that allowed the malicious traffic to reach the internal network
- Disruption of network services and resources
- Abnormal ICMP traffic patterns
- The need for improved traffic filtering and monitoring

Security measures identified during the investigation included:

- ICMP rate limiting
- Source IP address verification
- Network traffic monitoring
- IDS/IPS implementation
- Network and firewall log analysis

---

## Analysis

### Identify

The organization's network services and network resources were affected by the ICMP flood.

The misconfigured firewall was involved in the incident because it allowed malicious ICMP traffic to reach the internal network.

Critical network services were affected, while non-critical services were taken offline during the response.

### Protect

The organization implemented additional controls to reduce the risk of similar attacks.

These included:

- Firewall rules limiting the rate of incoming ICMP packets
- Source IP address verification to help detect and block IP spoofing
- IDS/IPS capabilities to filter suspicious ICMP traffic
- Improved firewall configuration

### Detect

Continuous network monitoring can be used to identify abnormal traffic patterns and potential security incidents.

Detection mechanisms included:

- Network traffic analysis
- IDS/IPS monitoring
- Source IP verification
- Security logs and alerts
- SIEM-based analysis of network events

These controls can help identify abnormal ICMP traffic and other suspicious activity.

### Respond

The response process focuses on containing and analyzing the incident.

The response actions included:

- Isolating affected systems
- Blocking malicious or suspicious ICMP traffic
- Analyzing firewall and network logs
- Identifying the characteristics and source of the attack
- Communicating the incident to relevant stakeholders
- Reviewing response procedures to identify improvements

### Recover

Recovery focuses on safely restoring affected services.

The recovery process included:

- Restoring critical network services first
- Verifying that restored services were functioning normally
- Gradually bringing non-critical services back online
- Monitoring network performance during restoration
- Reviewing and improving recovery procedures based on lessons learned

---

## Skills Demonstrated

- NIST Cybersecurity Framework (NIST CSF)
- Incident response
- Network security
- Denial-of-Service (DoS) analysis
- ICMP flood analysis
- Firewall security
- Network traffic monitoring
- IDS/IPS concepts
- IP spoofing detection
- SIEM concepts
- Incident containment
- Service recovery
- Security incident documentation

---

## Report

The complete incident report analysis is available below.

[View Incident Report](./incident-report.pdf)
