![Background](https://tryhackme-images.s3.amazonaws.com/user-uploads/5efe36fb68daf465530ca761/room-content/03376575e888fd097280c51469c29fbc.png)

<img src="https://tryhackme-images.s3.amazonaws.com/room-icons/55de4f7624252f03317e8e202822a6af.png" width="200" height="200" align="left">

# File Inclusion

**This room introduces file inclusion vulnerabilities, including Local File Inclusion (LFI), Remote File Inclusion (RFI), and directory traversal.**

**If you want to check out the room [click here](https://tryhackme.com/room/fileinc)**

---

**Table of Contents**

- [File Inclusion](#file-inclusion)
  - [Task 1 Introduction](#task-1-introduction)
  - [Task 2 Deploy the VM](#task-2-deploy-the-vm)
  - [Task 3 Path Traversal](#task-3-path-traversal)
  - [Task 4 Local File Inclusion - LFI](#task-4-local-file-inclusion---lfi)
  - [Task 5 Local File Inclusion - LFI #2](#task-5-local-file-inclusion---lfi-2)
  - [Task 6 Remote File Inclusion - RFI](#task-6-remote-file-inclusion---rfi)
  - [Task 7 Remediation](#task-7-remediation)
  - [Task 8 Challenge](#task-8-challenge)

## Task 1 Introduction

**Let's continue to the next section to deploy the attached VM.**

    No answer needed

## Task 2 Deploy the VM

**Once you've deployed the VM, please wait a few minutes for the webserver to start, then progress to the next section!**

    No answer needed

## Task 3 Path Traversal

**What function causes path traversal vulnerabilities in PHP?**

    file_get_contents

## Task 4 Local File Inclusion - LFI

**Give Lab #1 a try to read /etc/passwd. What would the request URI be?**

    lab1.php?file=/etc/passwd

**In Lab #2, what is the directory specified in the include function?**

    includes/

## Task 5 Local File Inclusion - LFI #2

**Give Lab #3 a try to read /etc/passwd. What is the request look like?**

    lab3.php?file=../../../../etc/passwd%00

**Which function is causing the directory traversal in Lab #4?**

    file_get_contents

**Try out Lab #6 and check what is the directory that has to be in the input field?**

    THM-profile

**Try out Lab #6 and read /etc/os-release. What is the VERSION_ID value?**

    12.04

## Task 6 Remote File Inclusion - RFI

**We showed how to include PHP pages via RFI. Do research on how to get remote command execution (RCE), and answer the question in the challenge section.**

    No answer needed

## Task 7 Remediation

**Ready for the challenges?**

    No answer needed

## Task 8 Challenge

**Capture Flag1 at /etc/flag1**

    ❗ This question cannot be given in accordance with TryHackMe's rules for submitting writeups for the room

**Capture Flag2 at /etc/flag2**

    ❗ This question cannot be given in accordance with TryHackMe's rules for submitting writeups for the room

**Capture Flag3 at /etc/flag3**

    ❗ This question cannot be given in accordance with TryHackMe's rules for submitting writeups for the room

**Gain RCE in Lab #Playground /playground.php with RFI to execute the hostname command. What is the output?**
