# reconnaissance-checklist
A streamlined reconnaissance checklist for bug bounty and pentesting workflows. Covers subdomain discovery, port scanning, HTTP probing, visual fingerprinting, parameter analysis, and automation tips. Designed for clean, modular, and scalable recon pipelines.

**AGGRESSIVE‑MODE RECON CHECKLIST**
A structured, high‑coverage, high‑intensity reconnaissance workflow for authorized security assessments.

**Pre‑Engagement Setup**

[ ] Confirm scope, rules of engagement, and authorization

[ ] Prepare resolvers list

[ ] Prepare wordlists (SecLists, Assetnote, custom)

[ ] Create project directory structure

[ ] Document all target domains, IPs, and cloud assets

Passive Reconnaissance (Stealth Phase)
Collect maximum intelligence without touching the target directly.

**Domain Intelligence**

[ ] WHOIS domain lookup

[ ] WHOIS IP ownership lookup

[ ] Identify registrant organization

[ ] Identify hosting provider

[ ] Identify ASN and IP ranges

**DNS Intelligence**

[ ] Query A, AAAA, NS, MX, TXT, SOA records

[ ] Identify DNS misconfigurations

[ ] Identify mail servers

[ ] Identify IPv6 presence

**Email & Contact OSINT**

[ ] Harvest public emails

[ ] Identify leaked credentials (public OSINT only)

[ ] Identify employee naming patterns

**Cloud & Infrastructure OSINT**

[ ] Identify cloud provider

[ ] Identify CDN usage

[ ] Identify hosting regions

[ ] Identify public buckets (OSINT only)

**Search Engine & Archive OSINT**

[ ] Identify indexed pages

[ ] Identify cached pages

[ ] Identify historical snapshots

[ ] Identify exposed directories

**WAF & Security Posture**

[ ] Detect WAF presence

[ ] Identify WAF vendor

[ ] Identify filtering behavior

**Subdomain Enumeration**
Combine multiple sources for maximum discovery.

**Passive Enumeration**

[ ] Certificate transparency

[ ] Public datasets

[ ] GitHub/GitLab enumeration

[ ] Analytics‑based enumeration

**Active Enumeration**

[ ] DNS brute‑forcing

[ ] Permutation‑based discovery

[ ] Wordlist‑based discovery

**Consolidation**

[ ] Merge all results

[ ] Deduplicate

[ ] Filter invalid domains

**DNS Resolution**
[ ] Resolve all subdomains

[ ] Validate DNS responses

[ ] Detect wildcard DNS

[ ] Identify takeover candidates

[ ] Identify stale DNS records

**Live Host Detection**

Identify every reachable asset.

[ ] Probe HTTP/HTTPS

[ ] Extract status codes

[ ] Extract titles

[ ] Detect technologies

[ ] Detect CDN

[ ] Detect IP addresses

[ ] Identify interesting ports (manual, controlled)

**URL & Content Discovery**
Collect every reachable endpoint.

**Live Crawling**

[ ] Crawl with depth control

[ ] Extract JS files

[ ] Extract endpoints

[ ] Extract forms

**Archive Crawling**

[ ] Collect historical URLs

[ ] Collect parameterized URLs

[ ] Collect hidden endpoints

**Consolidation**

[ ] Normalize URLs

[ ] Deduplicate

[ ] Filter noise

**JavaScript & Endpoint Analysis**

Extract maximum intelligence from JS files.

[ ] Extract endpoints

[ ] Extract secrets

[ ] Identify API routes

[ ] Identify hidden parameters

[ ] Identify sensitive keywords

[ ] Identify source maps

**Parameter Discovery**
[ ] Extract parameters from URLs

[ ] Generate permutations

[ ] Identify reflection points

[ ] Identify injection points

[ ] Identify dynamic parameters

**Behavior Analysis**

Understand how the application reacts to unusual inputs.

[ ] 403/401 bypass behavior

[ ] Cache poisoning behavior

[ ] Path traversal behavior

[ ] CRLF behavior

[ ] XSS reflection behavior

[ ] Rate‑limit behavior

[ ] Redirect behavior

**Fuzzing (Manual, Controlled, High‑Signal)**

Targeted fuzzing only — no blind blasting.

[ ] Directory fuzzing

[ ] Vhost fuzzing

[ ] Parameter fuzzing

[ ] Wordlist‑based probing

[ ] Technology‑specific fuzzing

**Vulnerability Scanning**

Use scanners as assistants, not as primary tools.

[ ] Run safe templates

[ ] Run tech‑specific templates

[ ] Run custom templates

[ ] Review all findings manually

[ ] Validate all findings manually

**Reporting & Documentation**

[ ] Deduplicate findings

[ ] Sort by severity

[ ] Document reproduction steps

[ ] Document impact

[ ] Document remediation

[ ] Prepare final report

[ ] Archive project data
