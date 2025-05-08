# Nmap (TryHackMe)

🔗 Room Name: Nmap  
🧠 Difficulty: Easy  
📁 Category: Network Scanning

---

## 📝 Overview

This room provides hands-on experience with `nmap`, the most widely used network scanning tool in cybersecurity. It covers basic and advanced scan types, script usage, firewall evasion, and interpreting scan results.

---

## 🛠️ Tools & Techniques Used

- `nmap`
- UDP, SYN, NULL, FIN, Xmas scans
- Nmap Scripting Engine (NSE)
- Firewall evasion techniques
- ICMP network scanning

---

## 🧪 Learning Objectives

- Perform different types of port scans and understand their use cases
- Use NSE scripts to gather more detailed information about services
- Identify hosts using ping scans (ICMP)
- Bypass basic firewall protections

---

## 🔍 Key Techniques Practiced

### ✅ Common Nmap Scan Types

```bash
nmap -sS target-ip        # SYN scan (stealthy and fast)
nmap -sU target-ip        # UDP scan
nmap -sN target-ip        # NULL scan
nmap -sF target-ip        # FIN scan
nmap -sX target-ip        # Xmas scan
```

### ✅ Script Scanning

```bash
nmap -sC target-ip        # Default scripts
nmap --script=http-enum target-ip
```

### ✅ Firewall Evasion

```bash
nmap -D RND:5 target-ip        # Decoy scan
nmap -f target-ip              # Fragment packets
nmap --source-port 53 target-ip  # Spoof source port
```

### ✅ ICMP Network Scanning

```bash
nmap -sn 192.168.1.0/24        # Ping scan
```

---

## 🎯 Key Takeaways

- Nmap is versatile for stealth, aggressive, and custom scans.
- Scripted scans can automate service enumeration.
- Evasion techniques are useful but should be used ethically and responsibly.
- Choosing the right scan type depends on the network defenses and your goal.

---

## ⚠️ Ethical Notice

This writeup is for educational purposes only. It respects the rules of TryHackMe and does not reveal solutions or flags.
