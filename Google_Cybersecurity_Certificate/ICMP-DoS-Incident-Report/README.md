
# **ICMP DoS Attack – Incident Report Analysis**

This case study analyzes a Denial‑of‑Service (DoS) attack caused by a flood of ICMP packets entering the organization’s network through an improperly configured firewall. The attack disrupted internal network services for two hours until the security team contained and resolved the issue. The report follows the NIST Cybersecurity Framework functions: Identify, Protect, Detect, Respond, and Recover.

## **Key Skills Demonstrated**
- Incident response documentation  
- Understanding of ICMP‑based DoS attacks  
- Firewall misconfiguration analysis  
- NIST CSF application  
- Network monitoring and detection strategies  
- Clear technical communication  

## **Tools / Concepts Used**
- ICMP packet analysis  
- Firewall rule configuration  
- IDS/IPS detection  
- Network monitoring  
- Incident response lifecycle  

## **Incident Summary**
- The organization experienced a DoS attack that caused internal services to stop responding.  
- A flood of ICMP packets overwhelmed the network due to an unconfigured firewall rule.  
- Normal internal traffic could not reach network resources during the attack.

## **NIST CSF Breakdown**

### **Identify**
A malicious actor exploited an unconfigured firewall, sending a high volume of ICMP pings that overwhelmed the network.

### **Protect**
- Implemented rate‑limiting for incoming ICMP packets  
- Enabled source IP verification to detect spoofed addresses  
- Scheduled regular firewall configuration reviews  

### **Detect**
- Added network monitoring tools to identify abnormal traffic patterns  
- Deployed IDS/IPS rules to filter suspicious ICMP traffic  

### **Respond**
- Blocked incoming ICMP packets  
- Took non‑critical services offline to stabilize the network  
- Restored critical services and documented all actions  

### **Recover**
- Restored all services after confirming network stability  
- Verified firewall changes  
- Monitored post‑incident traffic to ensure no recurrence  

## **Reflections**
- Regular firewall audits are essential  
- Quick response minimized downtime  
- Better baseline traffic monitoring is needed  
- Firewall configuration documentation must be improved  

## **Full Report**
See the attached PDF in this folder.

---

