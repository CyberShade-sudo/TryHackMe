# Nmap Live Host Discovery (TryHackMe)

🔗 Room Name: Nmap Live Host Discovery  
🧠 Difficulty: Easy  
📁 Category: Network Scanning

---

## 📝 Overview

This room focuses on identifying **live hosts** in a network using various Nmap host discovery techniques. It covers fundamental concepts like subnetting, ARP and ICMP-based discovery, TCP/UDP probing, and reverse DNS lookups.

---

## 🛠️ Tools & Techniques Used

- Subnetworks and CIDR notation
- Nmap ARP host discovery
- ICMP echo requests
- TCP/UDP host discovery methods
- Reverse DNS lookup

---

## 🧪 Learning Objectives

- Understand the importance of host discovery before port scanning
- Learn how to scan networks for active devices using Nmap
- Recognize the advantages and limitations of different discovery methods
- Perform reverse DNS lookups with Nmap

---

## 🔍 Key Techniques Practiced

### ✅ Subnetwork Scanning

```bash
nmap -sn 192.168.1.0/24
```

### ✅ ARP Discovery (on local network)

```bash
nmap -PR 192.168.1.0/24
```

### ✅ ICMP Discovery

```bash
nmap -PE 192.168.1.0/24
```

### ✅ TCP/UDP Host Discovery

```bash
nmap -PS22,80,443 192.168.1.0/24    # TCP SYN ping
nmap -PU53,161 192.168.1.0/24       # UDP ping
```

### ✅ Reverse DNS Lookup

```bash
nmap -sL 192.168.1.0/24
```

---

## 🎯 Key Takeaways

- ARP scanning is the most reliable on local networks.
- ICMP can be blocked by firewalls, so TCP/UDP scans may be used as alternatives.
- Reverse DNS is useful for passive mapping, but not always accurate.
- Efficient host discovery reduces scan time and noise.

---

## ⚠️ Ethical Notice

This writeup is for educational purposes only. It respects the rules of TryHackMe and does not reveal solutions or flags.
