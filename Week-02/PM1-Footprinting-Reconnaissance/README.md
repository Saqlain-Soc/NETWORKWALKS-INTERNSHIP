
# Week 2 – PM1: Footprinting & Reconnaissance

## Objective

Perform footprinting and reconnaissance on `networkwalks.com` using multiple Kali Linux tools and collect publicly available information about the target domain.

## Target

* Domain: `networkwalks.com`
* Platform: Kali Linux
* Purpose: Educational / Ethical Hacking

## Tasks

### Task 1 – WHOIS

```bash
whois networkwalks.com
```

Find domain registration details, registrar information, registration/expiry dates, and name servers.

### Task 2 – WhatWeb

```bash
whatweb networkwalks.com
```

Fingerprint the technologies used by the website, including web server, CMS, plugins, frameworks, and related information.

### Task 3 – NSLookup

```bash
nslookup networkwalks.com
```

Resolve the domain name and identify its associated IP address.

### Task 4 – CURL

```bash
curl -I https://networkwalks.com
```

Inspect HTTP response headers and related server information.

### Task 5 – WAFW00F

```bash
wafw00f networkwalks.com
```

Detect whether a Web Application Firewall (WAF) is protecting the website.

### Task 6 – DNSRecon

```bash
dnsrecon -d networkwalks.com
```

Enumerate publicly available DNS records, including name servers, mail servers, TXT/SPF and service records.

## Evidence

Screenshots and command outputs will be added after completing each task.

## Learning Outcome

This module provides practical experience with reconnaissance and footprinting techniques and demonstrates how publicly available domain, DNS, web technology, HTTP header, and WAF information can be collected during the reconnaissance phase of an ethical hacking assessment.

## Internship Information

* **Internship:** NetworkWALKS
* **Week:** 2
* **Module:** PM1
* **Topic:** Footprinting & Reconnaissance Attacks
