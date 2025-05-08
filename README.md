# Active Reconnaissance (TryHackMe)

🔗 Room Name: Active Reconnaissance  
🧠 Difficulty: Easy  
📁 Category: Information Gathering

---

## 📝 Overview

This room focuses on **active reconnaissance**, where interaction with the target system occurs to gather more detailed information. Unlike passive recon, this involves sending packets or making requests directly to the target.

---

## 🛠️ Tools Used

- Web Browser
- `ping`
- `traceroute`
- `telnet`
- `netcat (nc)`

---

## 🧪 Learning Objectives

- Understand the difference between passive and active recon
- Use basic network utilities to interact with and gather information from a target
- Recognize how network topology and services can be discovered through direct interaction

---

## 🔍 Key Techniques Practiced

### ✅ Ping

Used to check if a host is online and to measure latency:

```bash
ping target-ip
```

### ✅ Traceroute

Mapped the path packets take to a destination:

```bash
traceroute target-ip
```

### ✅ Telnet

Used to test open ports and banner grab services:

```bash
telnet target-ip 80
```

### ✅ Netcat

Utilized for port scanning and manual communication:

```bash
nc -v target-ip 80
```

---

## 🎯 Key Takeaways

- Active reconnaissance provides more detailed, real-time information but is detectable.
- Basic tools like `ping`, `traceroute`, and `telnet` are powerful for initial assessments.
- Understanding service banners and response behavior is essential for later phases like exploitation.

---

## ⚠️ Ethical Notice

This writeup is for educational purposes only. It respects the rules of TryHackMe and does not reveal solutions or flags.
