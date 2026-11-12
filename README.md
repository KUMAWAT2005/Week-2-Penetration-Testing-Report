# Week 2 – Penetration Testing Report

## Footprinting, Network Scanning & Vulnerability Assessment

**Cybersecurity Internship – Networkwalks**

**Author:** Ritesh Kumawat  
**Batch:** B084  
**Week:** 02  
**Date:** 12 November 2026

---

## 📌 Project Overview

This repository contains my Week 2 cybersecurity internship report, documenting practical activities related to footprinting, reconnaissance, and network scanning.

The practical work focuses on gathering publicly available information about a domain using Kali Linux tools and discovering active devices on a local network using Nmap and Zenmap.

Through these activities, I explored how cybersecurity professionals collect information, identify network devices, understand exposed technologies, and evaluate potential security risks.

## 🎯 Objectives

- Understand the footprinting and reconnaissance phases of penetration testing.
- Collect publicly available domain registration information.
- Identify website technologies and server information.
- Resolve domain names into IP addresses.
- Inspect HTTP response headers.
- Identify Web Application Firewall (WAF) technologies.
- Enumerate publicly available DNS records.
- Discover active devices on a local network.
- Identify IP and MAC address information where available.
- Understand basic network topology and potential security risks.

## 🛠️ Tools & Technologies Used

| Tool | Purpose |
|---|---|
| Kali Linux | Cybersecurity testing environment |
| WHOIS | Domain registration information |
| WhatWeb | Website technology fingerprinting |
| Nslookup | DNS lookup and IP resolution |
| Curl | HTTP response header inspection |
| Wafw00f | Web Application Firewall detection |
| DNSRecon | DNS record enumeration |
| Nmap | Network discovery and scanning |
| Zenmap | Graphical interface for Nmap |
| Windows CMD | Local IP and network configuration |

## 🔍 Practical Activities Performed

### 1. Footprinting & Reconnaissance

I used six Kali Linux tools to collect information about the `networkwalks.com` domain.

**Activity 1: WHOIS – Domain Registration**

Command:

```bash
whois networkwalks.com
```

Purpose:
- Identify domain registration information.
- Check registrar details.
- Observe domain creation information and name servers.

**Activity 2: WhatWeb – Technology Fingerprinting**

Command:

```bash
whatweb networkwalks.com
```

Purpose:
- Identify website technologies.
- Detect CMS information.
- Observe server and plugin details.

**Activity 3: Nslookup – DNS Resolution**

Command:

```bash
nslookup networkwalks.com
```

Purpose:
- Resolve the domain name into an IP address.
- Observe DNS server information.

**Activity 4: Curl – HTTP Header Inspection**

Command:

```bash
curl -I https://networkwalks.com
```

Purpose:
- Inspect HTTP response headers.
- Observe HTTP status information.
- Identify publicly exposed technical information.

**Activity 5: Wafw00f – WAF Detection**

Command:

```bash
wafw00f networkwalks.com
```

Purpose:
- Check whether a Web Application Firewall can be identified.
- Observe WAF technology information.

**Activity 6: DNSRecon – DNS Enumeration**

Command:

```bash
dnsrecon -d networkwalks.com
```

Purpose:
- Enumerate available DNS records.
- Identify name server and mail server information.
- Observe TXT and service-related records.

### 2. Network Scanning with Zenmap

The second practical activity focused on discovering active devices on my local network.

**Step 1: Identify Local IP Address**

Command:

```bash
ip a
```

Purpose:
- Identify the local IP address.
- Understand the network interface configuration.
- Determine the subnet.

**Step 2: Perform Network Discovery**

Command:

```bash
nmap -sn 10.0.0.0/24
```

Purpose:
- Discover active hosts.
- Identify available IP addresses.
- Observe MAC addresses where available.

**Step 3: Network Topology**

Using Zenmap, I explored the discovered hosts in the Topology section and documented the network layout.

This helped me understand how network discovery can be used to map devices within a local network.

## 📊 Key Findings Documented

The report records the following observations:

| Activity | Observation |
|---|---|
| WHOIS | Domain registration and name server information |
| WhatWeb | WordPress, WP Download Manager and Apache information |
| Nslookup | Resolved IP: `192.232.216.135` |
| Curl | HTTP response headers and WordPress REST API endpoint |
| Wafw00f | ModSecurity (SpiderLabs) identified |
| DNSRecon | DNS, mail server and TXT record information |
| Zenmap | Three live hosts documented on the local network |

**Note:** These are observations recorded in the report, not independently verified current results. They should be checked against your own practical evidence before submission.

## ⚠️ Risk Analysis

Based on the observations documented in the report, the following potential risks were considered:

| Potential Risk | Risk Level |
|---|---|
| Publicly exposed web technology information | Medium |
| Identifiable server IP address | Low |
| Exposed HTTP technical information | Low |
| Identifiable WAF technology | Low |
| Public DNS infrastructure information | Medium |
| Multiple visible live network hosts | Medium |

These findings represent potential information-disclosure and network-exposure risks. They are not confirmed vulnerabilities.

No exploitation or vulnerability validation is documented in these practical activities.

## 🔐 Security Recommendations

1. Regularly review publicly exposed website technology information.
2. Keep WordPress, themes, plugins and server software updated.
3. Review HTTP response headers and minimize unnecessary information disclosure.
4. Regularly review DNS records.
5. Keep the Web Application Firewall properly configured and monitored.
6. Perform authorized internal network discovery.
7. Investigate unknown or unauthorized devices.
8. Maintain updated network documentation.
9. Conduct security testing only with proper authorization.

## 📸 Evidence & Documentation

The project report includes practical evidence covering:

- WHOIS lookup
- WhatWeb technology fingerprinting
- Nslookup DNS resolution
- Curl HTTP header inspection
- Wafw00f detection
- DNSRecon enumeration
- Local network IP configuration
- Zenmap Ping Scan
- Zenmap network topology

The complete report is available in this repository as a PDF document.

## 📚 Learning Outcomes

Through this Week 2 practical work, I developed an understanding of:

- Footprinting and reconnaissance methodologies.
- Domain registration and DNS information gathering.
- Website technology fingerprinting.
- HTTP response header inspection.
- Web Application Firewall identification.
- DNS record enumeration.
- Network host discovery using Nmap.
- Network topology visualization using Zenmap.
- Security risk identification and reporting.

## ⚖️ Disclaimer

This project is intended strictly for educational and cybersecurity learning purposes.

All reconnaissance and network scanning activities must be performed only against systems and networks that you own or have explicit authorization to assess.

Unauthorized access, scanning or testing may violate applicable laws and regulations.

The author is not responsible for misuse of the information provided in this repository.

## 📖 References

- Kali Linux: https://www.kali.org/
- Nmap / Zenmap: https://nmap.org/
- WHOIS Lookup: https://who.is/
- Networkwalks: https://networkwalks.com/

## 👤 Author

**Ritesh Kumawat**  
Cybersecurity Student | Networkwalks B084

- **GitHub:** https://github.com/KUMAWAT2005
- **LinkedIn:** https://www.linkedin.com/in/ritesh-kumawat-0a430838a/

---

**Program:** Cybersecurity Internship – Networkwalks  
**Week:** 02  
**Project:** Footprinting, Network Scanning & Vulnerability Assessment

⭐ Thank you for visiting my repository!
