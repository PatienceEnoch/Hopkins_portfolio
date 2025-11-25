# 🟣 Tor Middle Relay Deployment  
### A Hands-On Networking & Security Engineering Project  
**Project Name:** CacheMeOutside (Middle Relay)  
**Platform:** Kali Linux VM  
**Category:** Network Engineering • Cybersecurity • Linux Administration

---

## 📌 Overview
This project involved deploying and operating a Tor middle relay as part of my hands-on networking and security engineering practice.  
A Tor relay is a node that helps route encrypted traffic through the Tor network, enabling multi-hop, privacy-preserving communications.

Running a middle relay (not an exit) is:
- safe  
- legal  
- an excellent networking lab  
- a real-world example of distributed routing + uptime management  

This project strengthened my understanding of routing, encryption circuits, Linux services, firewalls, public keys, and real-time network monitoring.

---

## 🎯 Objectives
- Deploy a fully functioning Tor middle relay  
- Learn how Tor builds encrypted multi-hop circuits  
- Configure and manage a public-facing network service  
- Work with systemd, logs, keys, and reachability testing  
- Monitor performance and health through Tor Metrics  

---

## 🛠 Technologies & Skills Used
- Linux Administration (Kali Linux)  
- Networking: ORPorts, firewalls, reachability checks  
- Systemd (systemctl, service management)  
- Encryption & Key Management (/var/lib/tor/keys/)  
- Routing & Privacy Engineering Concepts  
- Distributed Systems Monitoring  
- Public Relay Identity (Fingerprint)  

---

## 📡 Relay Deployment Summary

### Relay Nickname  
CacheMeOutside

### Fingerprint  
6C107E82F0BA26F2BEB3F5745BEC7F033ABDCA94

### ORPort & Reachability  
Relay successfully reached by directory authorities via:  
<REDACTED_IP>:9001

### Relay Type  
✔ Middle Relay  
✘ Exit Relay (safe setup)

### Initial Flags Received
- Running  
- Valid  
- V2Dir  

---

## 🧩 Configuration (torrc)
Below is a sanitized version of the relay’s torrc configuration:

```
Nickname CacheMeOutside
ORPort 9001
DirPort 9030
SocksPort 0
ExitRelay 0
ExitPolicy reject *:*
ContactInfo <email redacted>
Log notice file /var/log/tor/notices.log
```

---

## 🔍 Monitoring & Metrics
Relay was verified using Tor Metrics:  
- Uptime  
- Flags  
- Reachability  
- Advertised bandwidth  
- Consensus weight  

All indicators showed a healthy, functioning middle relay.

---

## 💡 What I Learned
- How Tor constructs anonymized circuits  
- Why multi-hop encrypted routing requires public relays  
- Managing long-running Linux services  
- Reading logs and diagnosing reachability issues  
- Core Linux topics: permissions, ownership, system services  
- The structure of the Tor directory authority system  
- How uptime affects relay selection weight  

This project deepened my understanding of network infrastructure, anonymity networks, distributed systems, and encrypted routing.

---

## 🚀 Next Steps
- Continue uptime to earn additional relay flags  
- Automate deployment with Ansible or Terraform (advanced)  
- Deploy a second relay in my lab network  
- Set up Tor relay dashboards or Prometheus metrics  

---

## 📁 Screenshots  
(Add redacted screenshot here once uploaded)

---

## 📎 Final Thoughts
Running a Tor middle relay was an excellent way to apply cloud/network engineering concepts in a real-world environment.  
This project strengthened my skills in Linux, routing, privacy engineering, and service reliability.
