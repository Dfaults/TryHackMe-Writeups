![Background](https://assets.tryhackme.com/additional/dnsindetail/dnsindetail.png)

<img src="https://tryhackme-images.s3.amazonaws.com/room-icons/64e64795aa420cc8e9fb3be1bd69c302.png" width="200" height="200" align="left">

# DNS in detail

##### In this room we see an overview of how DNS works along with identifyng each of it's parts.

##### If you want to check out the room [click here](https://tryhackme.com/room/dnsindetail)

#

### Table of Contents

- [DNS in detail](#dns-in-detail)
        - [In this room we see an overview of how DNS works along with identifyng each of it's parts.](#in-this-room-we-see-an-overview-of-how-dns-works-along-with-identifyng-each-of-its-parts)
        - [If you want to check out the room click here](#if-you-want-to-check-out-the-room-click-here)
    - [Table of Contents](#table-of-contents)
- [Task 1 What is DNS?](#task-1-what-is-dns)
    - [What does DNS stand for?](#what-does-dns-stand-for)
- [Task 2 Domain Hierarchy](#task-2-domain-hierarchy)
    - [What is the maximum length of a subdomain?](#what-is-the-maximum-length-of-a-subdomain)
    - [Which of the following characters cannot be used in a subdomain ( 3 b _ - )?](#which-of-the-following-characters-cannot-be-used-in-a-subdomain--3-b-_---)
    - [What is the maximum length of a domain name?](#what-is-the-maximum-length-of-a-domain-name)
    - [What type of TLD is .co.uk?](#what-type-of-tld-is-couk)
- [Task 3 Record Types](#task-3-record-types)
    - [What type of record would be used to advise where to send email?](#what-type-of-record-would-be-used-to-advise-where-to-send-email)
    - [What type of record handles IPv6 addresses?](#what-type-of-record-handles-ipv6-addresses)
- [Task 4 Making a Request](#task-4-making-a-request)
    - [What field specifies how long a DNS record should be cached for?](#what-field-specifies-how-long-a-dns-record-should-be-cached-for)
    - [What type of DNS Server is usually provided by your ISP?](#what-type-of-dns-server-is-usually-provided-by-your-isp)
    - [What type of server holds all the records for a domain?](#what-type-of-server-holds-all-the-records-for-a-domain)
- [Task 5 Practical](#task-5-practical)
    - [What is the CNAME of shop.website.thm?](#what-is-the-cname-of-shopwebsitethm)
    - [What is the value of the TXT record of website.thm?](#what-is-the-value-of-the-txt-record-of-websitethm)
    - [What is the numerical priority value for the MX record?](#what-is-the-numerical-priority-value-for-the-mx-record)
    - [What is the IP address for the A record of www.website.thm?](#what-is-the-ip-address-for-the-a-record-of-wwwwebsitethm)

# Task 1 What is DNS?

### What does DNS stand for?

    Domain Name System

# Task 2 Domain Hierarchy

### What is the maximum length of a subdomain?

    63

### Which of the following characters cannot be used in a subdomain ( 3 b _ - )?

    _

### What is the maximum length of a domain name?

    253

### What type of TLD is .co.uk?

    ccTLD

# Task 3 Record Types

### What type of record would be used to advise where to send email?

    MX

### What type of record handles IPv6 addresses?

    AAAA

# Task 4 Making a Request

### What field specifies how long a DNS record should be cached for?

    TTL

### What type of DNS Server is usually provided by your ISP?

    Recursive

### What type of server holds all the records for a domain?

    Authoritative

# Task 5 Practical

### What is the CNAME of shop.website.thm?

    shops.myshopify.com

### What is the value of the TXT record of website.thm?

    Can't be provided under THMs terms for submiting writeups in their rooms.

### What is the numerical priority value for the MX record?

    30

### What is the IP address for the A record of www.website.thm?

    10.10.10.10
