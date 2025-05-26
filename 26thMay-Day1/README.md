# 🔍 Nmap Scan Task

## 📌 Objective:

Perform a SYN scan using Nmap to identify open ports on the local system.

## 🛠️ Tools:

* Nmap 7.94SVN
* Linux (VirtualBox)

## 📝 Steps:

1. Found IP using:

   ```bash
   hostname -I
   ```

   → `10.0.2.15`

2. Ran SYN scan:

   ```bash
   sudo nmap -sS 10.0.2.15
   ```

## ✅ Result:

* Host is up
* Open ports:

  * **22/tcp** — SSH
  * **443/tcp** — HTTPS

## Outcome:
Learned to scan for open ports using Nmap, useful in network monitoring and SOC operations.
