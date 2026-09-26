# Network Traffic Analysis – TCP SYN Flood

## Overview

This project is a cybersecurity incident investigation completed as part
of the Google Cybersecurity Professional Certificate.

The objective was to analyze network traffic captured with Wireshark and
identify the cause of a web server availability issue.

## Scenario

Users were unable to access the company's website.

The browser returned a connection timeout error.

## Investigation

The Wireshark traffic showed:

- A large volume of TCP SYN packets
- SYN packets targeting the web server
- TCP connection attempts that were not successfully completed
- The web server becoming overwhelmed
- Legitimate users experiencing connection timeout errors

## Analysis

The evidence indicates that the web server was experiencing a TCP SYN
flood, a type of Denial-of-Service (DoS) attack.

The attacker sends a large number of SYN requests to the web server,
causing it to maintain numerous half-open TCP connections.

This can consume the server's available connection resources and fill
its TCP connection backlog, preventing legitimate clients from
establishing new connections.

Possible mitigations include:

- SYN cookies
- SYN rate limiting
- Firewall and IPS rules
- DDoS protection
- Network traffic monitoring

Further investigation would be required to determine the source and
full scope of the attack.

## Skills Demonstrated

- Network traffic analysis
- TCP/IP
- TCP three-way handshake
- Denial-of-Service (DoS) analysis
- Wireshark
- Incident reporting
- Network troubleshooting

## Report

[View the incident report](./tcp-syn-flood-incident-report.pdf)
