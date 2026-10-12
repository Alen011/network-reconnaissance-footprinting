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

- Collected domain registration information.
- Queried DNS records and checked common subdomains.
- Investigated publicly indexed pages using search operators.
- Tested host reachability and examined the network path.
- Identified exposed services and service versions with Nmap.
- Inspected HTTP response headers and web technologies.
- Documented findings, limitations, and potential follow-up checks.

## Key Findings

- Identified SSH and HTTP services during service/version detection.
- Observed Apache and OpenSSH version information indicating an Ubuntu-based environment.
- Collected DNS and mail-server information for the domain.
- Recorded limitations and inconsistencies that required further verification.

Version banners alone do not confirm that a service is vulnerable or unpatched.

## Deliverables

- Detailed project report with terminal screenshots, methodology, results, and conclusions.
- Documentation of tools used and limitations encountered.

## Scope & Ethics

Testing was limited to the authorized target and non-destructive reconnaissance. No exploitation or denial-of-service testing was performed.

## What I Learned

- Fundamental network reconnaissance and footprinting.
- DNS enumeration and service fingerprinting.
- Using command-line security tools in Kali Linux.
- Interpreting scan results cautiously and documenting technical findings.

---

**Author:** Alen Shibu  
**Project:** InternVision Cyber Security Internship
