<img src="https://tryhackme-images.s3.amazonaws.com/room-icons/9a88b741fd89551e0e041d3021c8ad8f.png" width="100" height="100" align="left">

# Network Security Solutions

### Learn about and experiment with various IDS/IPS evasion techniques, such as protocol and payload manipulation

#

### Table of Contents


- [Network Security Solutions](#network-security-solutions)
    - [Learn about and experiment with various IDS/IPS evasion techniques, such as protocol and payload manipulation](#learn-about-and-experiment-with-various-idsips-evasion-techniques-such-as-protocol-and-payload-manipulation)
    - [Table of Contents](#table-of-contents)
- [Task 1 Introduction](#task-1-introduction)
    - [What does an Ips stand for?](#what-does-an-ips-stand-for)
    - [What do you call a system that can detect malicious activity but not stop it?](#what-do-you-call-a-system-that-can-detect-malicious-activity-but-not-stop-it)
- [Task 2 IDS Engine Types](#task-2-ids-engine-types)
    - [What kind of IDS engine has a database of all known malicious packets’ contents?](#what-kind-of-ids-engine-has-a-database-of-all-known-malicious-packets-contents)
    - [What kind of IDS engine needs to learn what normal traffic looks like instead of malicious traffic?](#what-kind-of-ids-engine-needs-to-learn-what-normal-traffic-looks-like-instead-of-malicious-traffic)
    - [What kind of IDS engine needs to be updated constantly as new malicious packets and activities are discovered?](#what-kind-of-ids-engine-needs-to-be-updated-constantly-as-new-malicious-packets-and-activities-are-discovered)
- [Task 3 IDS/IPS Rule Triggering](#task-3-idsips-rule-triggering)
    - [In the attached file, the logs show that a specific IP address has been detected scanning our system of IP address {IP found in your machine here}. What is the IP address running the port scan?](#in-the-attached-file-the-logs-show-that-a-specific-ip-address-has-been-detected-scanning-our-system-of-ip-address-ip-found-in-your-machine-here-what-is-the-ip-address-running-the-port-scan)
- [Task 4 Evasion via Protocol Manipulation](#task-4-evasion-via-protocol-manipulation)
    - [We use the following Nmap command, nmap -sU -F MACHINE_IP, to launch a UDP scan against our target. What is the option we need to add to set the source port to 161?](#we-use-the-following-nmap-command-nmap--su--f-machine_ip-to-launch-a-udp-scan-against-our-target-what-is-the-option-we-need-to-add-to-set-the-source-port-to-161)
    - [The target allows Telnet traffic. Using ncat, how do we set a listener on the Telnet port?](#the-target-allows-telnet-traffic-using-ncat-how-do-we-set-a-listener-on-the-telnet-port)
    - [We are scanning our target using nmap -sS -F MACHINE_IP. We want to fragment the IP packets used in our Nmap scan so that the data size does not exceed 16 bytes. What is the option that we need to add?](#we-are-scanning-our-target-using-nmap--ss--f-machine_ip-we-want-to-fragment-the-ip-packets-used-in-our-nmap-scan-so-that-the-data-size-does-not-exceed-16-bytes-what-is-the-option-that-we-need-to-add)
    - [Which of the above three arguments would return meaningful results when scanning MACHINE_IP?](#which-of-the-above-three-arguments-would-return-meaningful-results-when-scanning-machine_ip)
    - [What is the option in hping3 to set a custom TCP window size?](#what-is-the-option-in-hping3-to-set-a-custom-tcp-window-size)
- [Task 5 Evasion via Payload Manipulation](#task-5-evasion-via-payload-manipulation)
- [Task 6 Evasion via Route Manipulation](#task-6-evasion-via-route-manipulation)
- [Task 7 Evasion via Tactical DoS](#task-7-evasion-via-tactical-dos)
- [Task 8 C2 and IDS/IPS Evasion](#task-8-c2-and-idsips-evasion)
- [Task 9 Next-Gen Security](#task-9-next-gen-security)
- [Task 10 Summary](#task-10-summary)

# Task 1 Introduction

### What does an Ips stand for?

    Intrusion Prevention System

### What do you call a system that can detect malicious activity but not stop it?

    Intrusion Detection System

# Task 2 IDS Engine Types

### What kind of IDS engine has a database of all known malicious packets’ contents?

    Signature-based

### What kind of IDS engine needs to learn what normal traffic looks like instead of malicious traffic?

    anomaly-based

### What kind of IDS engine needs to be updated constantly as new malicious packets and activities are discovered?

    signature-based

# Task 3 IDS/IPS Rule Triggering

### In the attached file, the logs show that a specific IP address has been detected scanning our system of IP address {IP found in your machine here}. What is the IP address running the port scan?

    {IP found in your machine here}

# Task 4 Evasion via Protocol Manipulation

### We use the following Nmap command, nmap -sU -F MACHINE_IP, to launch a UDP scan against our target. What is the option we need to add to set the source port to 161?

    -g 161

### The target allows Telnet traffic. Using ncat, how do we set a listener on the Telnet port?

    ncat -lvnp 23

### We are scanning our target using nmap -sS -F MACHINE_IP. We want to fragment the IP packets used in our Nmap scan so that the data size does not exceed 16 bytes. What is the option that we need to add?

    -ff

### Which of the above three arguments would return meaningful results when scanning MACHINE_IP?

    -sF

### What is the option in hping3 to set a custom TCP window size?

    -w

# Task 5 Evasion via Payload Manipulation

# Task 6 Evasion via Route Manipulation

# Task 7 Evasion via Tactical DoS

# Task 8 C2 and IDS/IPS Evasion

# Task 9 Next-Gen Security

# Task 10 Summary
