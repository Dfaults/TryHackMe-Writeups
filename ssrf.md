![Background](https://tryhackme-images.s3.amazonaws.com/user-uploads/5efe36fb68daf465530ca761/room-content/03376575e888fd097280c51469c29fbc.png)

<img src="https://tryhackme-images.s3.amazonaws.com/room-icons/268e10b8ee0b53d1074b2a7fd5b1a789.png" width="200" height="200" align="left">

# SSRF

**Learn how to exploit Server-Side Request Forgery (SSRF) vulnerabilities, allowing you to access internal server resources.**

**If you want to check out the room [click here](https://tryhackme.com/room/ssrfqi)**

---

<br>

**Table of Contents**

- [SSRF](#ssrf)
  - [Task 1](#task-1)
    - [Explanation](#explanation)
  - [Task 2](#task-2)
  - [Task 3](#task-3)
  - [Task 4](#task-4)
  - [Task 5](#task-5)
  - [Terminology](#terminology)

## Task 1

### Explanation

Server Side Request Forgery is a web vulnerability know for allowing the attacker to intentionally make requests to a location of the attackers choosing. This can lead to giving the attacker the option of using either server side only services or conect to an external resource already prepared for the engagement, thus permiting information disclosure or potentially and RCE[^RCE]. However, there is also the blind SSRF attack in which there is no output towards the attacker. In this case the suggested course of action would be to try and get a reverse connection back in order to proceed with gaining access. A typical attack may look like this in regards to a regular HTTP request sent towards a shopping store:

Regular request:

```http
POST /product/stock HTTP/1.0
Content-Type: application/x-www-form-urlencoded
Content-Length: 118

stockApi=http://stock.weliketoshop.net:8080/product/stock/check%3FproductId%3D6%26storeId%3D1
```

Forged request:

```http
POST /product/stock HTTP/1.0
Content-Type: application/x-www-form-urlencoded
Content-Length: 118

stockApi=http://localhost/admin
```

This forged request is sent because the trust given to the system itself is far greater than the one given to any user or in this case attacker, thus there is a higher likelyhood of bypassing the normal AC[^AC] controls.

**What does SSRF stand for?**

    Server Side Request Forgery

**As opposed to a regular SSRF, what is the other type?**

    Blind

## Task 2

**What is the flag from the SSRF Examples site?**

    ❗ This question cannot be given in accordance with TryHackMe's rules for submitting writeups for the room

> 💡**Tip:** Try slowly and calmy reading the instructions given for the challange, in order to get the flag you need to force the webserver request the site given and ignore the actual backend request. This can be done by utilizing one of the last techniques mentioned in the tutorial but pay special atention to the url that will give you the flag and don't add the "https://" when requesting the flag.

## Task 3

**What website can be used to catch HTTP requests from a server?**

    requestbin.com

> 💡 **Tip:** You can also check out [Cheat Sheets](https://0xn3va.gitbook.io/cheat-sheets/web-application/server-side-request-forgery) in order to see how to circumvent SSRF filters.

## Task 4

**What method can be used to bypass strict rules?**

    Open Redirect

**What IP address may contain sensitive data in a cloud environment?**

    169.254.169.254

**What type of list is used to permit only certain input?**

    Allow List

**What type of list is used to stop certain input?**

    Deny List

## Task 5

**What is the flag from the /private directory?**

    ❗ This question cannot be given in accordance with TryHackMe's rules for submitting writeups for the room

## Terminology

[^RCE]: **Remote Code Execution**
Refers to the act of running a custom or otherwise malitious script on a victim in order to get unintended execusion or access to it's resources.

[^AC]: **Access Control**
Refers to the system that's put in place in order to secure an application from unauthorized access. Normally these are positioned infront of a system or resource in order to protect it.
