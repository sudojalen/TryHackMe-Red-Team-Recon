# TryHackMe: Red Team Recon – Technical Lab Summary

## Project Overview

This project focused on the foundational phase of cyber operations: **Reconnaissance**. The goal was to master the techniques used to gather as much information as possible about a target to identify potential entry points and vulnerabilities. Following the philosophy of Sun Tzu, this lab emphasized that "knowing the enemy" begins with comprehensive data collection before launching any active attack.

## The Reconnaissance Process

The lab explored how to map an organization's digital footprint using both manual tools and automated frameworks. The focus was on expanding knowledge of the target's terrain to refine later attack phases, such as vulnerability scanning or phishing.

[Image of the reconnaissance phase of the cyber kill chain]

### 1. Built-in Network Utilities
I used several essential command-line tools to pull direct information from the target's infrastructure:
* **WHOIS:** Queried registration databases to find ownership details, such as administrative contacts and registration dates.
* **Dig:** Interrogated DNS servers to discover subdomains, mail servers (MX records), and IP addresses associated with the domain.
* **Traceroute (tracert):** Mapped the physical path packets take to reach the target, revealing the network's hop-by-hop structure and potential security hardware.

### 2. OSINT Automation Frameworks
Beyond manual queries, I utilized powerful platforms to aggregate and correlate large amounts of data:
* **Recon-ng:** A modular web reconnaissance framework used to automate the collection of subdomains, employee emails, and other public-facing data.
* **Maltego:** A graphical tool used to visualize complex relationships between different entities, such as how an IP address connects to a specific person or organization.

[Image of Maltego graph showing relationships between domains and IP addresses]

## Key Concepts Learned

* **Information Leveraging:** Understanding how simple data points (like an email address) can be used to launch sophisticated phishing campaigns or brute-force attacks.
* **Passive vs. Active Recon:** Learning the difference between gathering data from third-party sources (Passive) versus interacting directly with target servers (Active).
* **Target Expansion:** Identifying that the more information gathered, the higher the success rate for subsequent exploitation phases.

---

## Lab Evidence (Screenshots)

| Activity | Technical Goal | Screenshot Placeholder |
| :--- | :--- | :--- |
| **Domain Query** | Using `whois` and `dig` to find public assets. | `[Insert Screenshot Here]` |
| **Network Pathing** | Mapping network hops using `tracert`. | `[Insert Screenshot Here]` |
| **OSINT Correlation** | Using Maltego or Recon-ng to link data points. | `[Insert Screenshot Here]` |

---

## Technical Environment

* **Platform:** TryHackMe (AttackBox / Kali Linux)
* **Tools:** WHOIS, Dig, Traceroute, Recon-ng, Maltego
* **Source:** CrowdStrike (n.d.). *Reconnaissance Detection*. [https://www.crowdstrike.com/cybersecurity-101/red-teaming/reconnaissance-detection-blue-team/](https://www.crowdstrike.com/cybersecurity-101/red-teaming/reconnaissance-detection-blue-team/)
