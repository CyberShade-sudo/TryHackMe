# Passive Reconnaissance (TryHackMe)

🔗 Room Link: [Passive Reconnaissance](https://tryhackme.com/room/passiverecon)  
🧠 Difficulty: Easy  
📁 Category: Information Gathering

---

## 📝 Overview

This room introduces **passive reconnaissance** techniques—methods of gathering information without directly interacting with the target. It covers tools and services that help gather public information using Open Source Intelligence (OSINT).

---

## 🛠️ Tools & Resources Used

- Google Search Operators
- WHOIS Lookup
- NSLookup / Dig
- Shodan
- Certificate Transparency Logs (crt.sh)
- Wayback Machine (archive.org)
- Hunter.io
- Social media and blog searches

---

## 🧪 Learning Objectives

- Understand the difference between active and passive recon
- Discover domains, subdomains, and services using OSINT
- Explore email harvesting and DNS record gathering
- Learn about online footprint tracing

---

## 🔍 Key Techniques Practiced

### ✅ WHOIS Lookup

Used to identify domain ownership and registration data:

```bash
whois example.com
```

### ✅ DNS Record Discovery

Queried A, MX, TXT, and NS records:

```bash
nslookup -type=mx example.com
```

or

```bash
dig example.com ANY
```

### ✅ Shodan

Found open services exposed on the internet:

- Search: `org:"CompanyName"` or `ip:targetIP`

### ✅ Certificate Search

Found subdomains using:

- [crt.sh](https://crt.sh)
- [Censys](https://censys.io)

### ✅ Wayback Machine

Used to discover archived pages of a target website and exposed endpoints or technologies.

---

## 🎯 Key Takeaways

- Passive reconnaissance is legal and stealthy, useful for the first phase of a penetration test.
- Publicly available information can often reveal sensitive data, such as subdomains, email addresses, and even software versions.
- Tools like Shodan and crt.sh are powerful for mapping an organization’s external footprint.

---

## ⚠️ Ethical Notice

This writeup is for educational purposes only. No flags or answers are revealed in compliance with TryHackMe’s [Terms of Use](https://tryhackme.com/terms).
