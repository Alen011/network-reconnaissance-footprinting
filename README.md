# Network Reconnaissance & Footprinting

A cybersecurity project completed as part of the InternVision Cyber Security Internship, focused on authorized network reconnaissance and footprinting using Kali Linux.

## Project Overview

The objective was to gather publicly available information about a target domain and identify its network services and web technologies using passive information gathering and limited, authorized active probing.

## Target & Environment

- **Target:** `scanme.nmap.org`
- **Environment:** Kali Linux running in Oracle VirtualBox
- **Project type:** Cybersecurity minor project
- **Testing date:** October 8, 2026

Active scanning was restricted to `scanme.nmap.org`, a host provided by the Nmap Project for scan testing.

## Tools Used

| Tool | Purpose |
|---|---|
| WHOIS | Domain registration information |
| `dig` / `nslookup` | DNS record enumeration |
| Google Search operators | Publicly indexed information discovery |
| `ping` | Host reachability and latency |
| `traceroute` | Network path investigation |
| Nmap | Port scanning and service/version detection |
| `curl` | HTTP response header inspection |
| WhatWeb | Web technology fingerprinting |

## Work Performed

- Collected domain registration information using WHOIS.
- Queried DNS records, including address and mail-exchange records.
- Performed preliminary checks for common subdomains; results were not independently verified as valid subdomains.
- Investigated publicly indexed pages using Google Search operators.
- Tested host reachability and examined the network path using `ping` and `traceroute`.
- Performed Nmap service/version detection against the target.
- Inspected HTTP response headers using `curl` and identified web technologies using WhatWeb.
- Documented findings, limitations, and areas requiring further verification.

## Key Findings

- Nmap service/version detection identified SSH (port `22/tcp`) and HTTP (port `80/tcp`) as open among the 100 most common TCP ports scanned.
- The remaining 98 scanned TCP ports were reported as filtered. This result applies only to the scanned ports and does not establish the state of every port on the host.
- Service banners identified OpenSSH `6.6.1p1` and Apache HTTP Server `2.4.7` on Ubuntu.
- DNS queries returned address records for `scanme.nmap.org` and mail-exchange records for `nmap.org`.
- WHOIS queries provided domain registration and nameserver information.
- HTTP response headers provided additional information about the web server.
- WhatWeb identified web technologies over HTTP. The HTTPS connection attempt was refused, so HTTPS availability was not confirmed.
- The preliminary subdomain checks returned matching IP addresses, but these results alone did not establish that the tested names were valid subdomains.

Version banners and service identification alone do not confirm that a service is vulnerable or unpatched. Further verification would be required before drawing security conclusions.

## Deliverables

- Detailed project report containing the methodology, terminal screenshots, results, and conclusions.
- Documentation of the tools used, observations, and limitations.
- Selected screenshots demonstrating the reconnaissance workflow.

## Scope & Ethics

Testing was limited to the designated Nmap scan-testing target and non-destructive reconnaissance activities. No exploitation or denial-of-service testing was performed.

The results represent observations from the testing date and may change as the target's configuration or services change.

## What I Learned

- Fundamental network reconnaissance and footprinting techniques.
- DNS enumeration and service fingerprinting.
- Using command-line security tools in Kali Linux.
- Interpreting Nmap results and HTTP responses.
- Recognizing the limitations of preliminary subdomain checks and service banners.
- Documenting technical findings clearly and responsibly.

---

Author: Alen Shibu  
Project: InternVision Cyber Security Internship
