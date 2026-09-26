# Network Traffic Analysis – DNS Incident

## Overview

This project is a cybersecurity incident investigation completed as part
of the Google Cybersecurity Professional Certificate.

The objective was to analyze network traffic captured with tcpdump and
identify the cause of a DNS-related connectivity issue.

## Scenario

Users were unable to access:

www.yummyrecipesforme.com

The browser returned a "Destination port unreachable" error.

## Investigation

The tcpdump traffic showed:

- DNS queries using UDP
- Destination port 53
- DNS server: 203.0.113.2
- ICMP Destination Unreachable responses
- Error: `udp port 53 unreachable`

## Analysis

The evidence indicates that the DNS service was unavailable or that
UDP port 53 was not accepting traffic.

Possible causes include:

- DNS service failure
- DNS configuration issue
- Firewall configuration

Further investigation would be required to identify the root cause.

## Skills Demonstrated

- Network traffic analysis
- DNS
- UDP
- ICMP
- tcpdump
- Incident reporting
- Network troubleshooting

## Report

[View the incident report](./incident-report.pdf)
