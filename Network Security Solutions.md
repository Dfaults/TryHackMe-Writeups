![Background](https://assets.tryhackme.com/room-banners/evasion.png)

<img src="https://tryhackme-images.s3.amazonaws.com/room-icons/9a88b741fd89551e0e041d3021c8ad8f.png" width="200" height="200" align="left">

# Network Security Solutions

**Learn about and experiment with various IDS/IPS evasion techniques, such as protocol and payload manipulation**

**If you want to check out the room [click here](https://tryhackme.com/room/redteamnetsec)**

---

<br>

**Table of Contents**

- [Network Security Solutions](#network-security-solutions)
- [Task 1 Introduction](#task-1-introduction)
- [Task 2 IDS Engine Types](#task-2-ids-engine-types)
- [Task 3 IDS/IPS Rule Triggering](#task-3-idsips-rule-triggering)
- [Task 4 Evasion via Protocol Manipulation](#task-4-evasion-via-protocol-manipulation)
- [Task 5 Evasion via Payload Manipulation](#task-5-evasion-via-payload-manipulation)
- [Task 6 Evasion via Route Manipulation](#task-6-evasion-via-route-manipulation)
- [Task 7 Evasion via Tactical DoS](#task-7-evasion-via-tactical-dos)
- [Task 8 C2 and IDS/IPS Evasion](#task-8-c2-and-idsips-evasion)
- [Task 9 Next-Gen Security](#task-9-next-gen-security)
- [Task 10 Summary](#task-10-summary)

---

# Task 1 Introduction

**What does an Ips stand for?**

    Intrusion Prevention System

**What do you call a system that can detect malicious activity but not stop it?**

    Intrusion Detection System

# Task 2 IDS Engine Types

**What kind of IDS engine has a database of all known malicious packets’ contents?**

    Signature-based

**What kind of IDS engine needs to learn what normal traffic looks like instead of malicious traffic?**

    anomaly-based

**What kind of IDS engine needs to be updated constantly as new malicious packets and activities are discovered?**

    signature-based

# Task 3 IDS/IPS Rule Triggering

**In the attached file, the logs show that a specific IP address has been detected scanning our system of IP address {IP found in your machine here}. What is the IP address running the port scan?**

    {IP found in your machine here}

# Task 4 Evasion via Protocol Manipulation

**We use the following Nmap command, nmap -sU -F MACHINE_IP, to launch a UDP scan against our target. What is the option we need to add to set the source port to 161?**

    -g 161

**The target allows Telnet traffic. Using ncat, how do we set a listener on the Telnet port?**

    ncat -lvnp 23

**We are scanning our target using nmap -sS -F MACHINE_IP. We want to fragment the IP packets used in our Nmap scan so that the data size does not exceed 16 bytes. What is the option that we need to add?**

    -ff

**Which of the above three arguments would return meaningful results when scanning MACHINE_IP?**

    -sF

**What is the option in hping3 to set a custom TCP window size?**

    -w

# Task 5 Evasion via Payload Manipulation

**Using base64 encoding, what is the transformation of cat /etc/passwd?**

    Y2F0IC9ldGMvcGFzc3dkCg==

**The base32 encoding of a particular string is NZRWC5BAFVWCAOBQHAYAU===. What is the original string?**

    ncat -l 8080

**Using the provided openssl command above. You created a certificate, which we gave the extension .crt, and a private key, which we gave the extension .key. What is the first line in the certificate file?**

    -----BEGIN CERTIFICATE-----

**What is the last line in the private key file?**

    -----END PRIVATE KEY-----

**On the attached machine from the previous task, browse to <http://MACHINE_IP:8080>, where you can write your Linux commands. Note that no output will be returned. A command like ncat -lvnp 1234 -e /bin/bash will create a bind shell that you can connect to it from the AttackBox using ncat MACHINE_IP 1234; however, some IPS is filtering out the command we are submitting on the form. Using one of the techniques mentioned in this task, try to adapt the command typed in the form to run properly. Once you connect to the bind shell using ncat MACHINE_IP 1234, find the user’s name**

    redteamnetsec
> Tip: When you run the command you won't get any obvious response in the listner terminal so just write commands directly in order to get the response needed to complete the task

# Task 6 Evasion via Route Manipulation

    http socks4

# Task 7 Evasion via Tactical DoS

    No answer needed

# Task 8 C2 and IDS/IPS Evasion

    jitter

# Task 9 Next-Gen Security

    No answer needed

# Task 10 Summary

    No answer needed
