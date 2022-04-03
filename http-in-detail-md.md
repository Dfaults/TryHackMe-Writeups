![Background](https://assets.tryhackme.com/additional/httpindetail/httpindetail.png)

<img src="https://tryhackme-images.s3.amazonaws.com/room-icons/fc8943a1ff801b60d586e165812212c6.png" width="200" height="200" align="left">

# HTTP in detail

##### Learn about how to request content from a web server using the HTTP protocol

##### If you want to check out the room [click here](https://tryhackme.com/room/dnsindetail)

#

### Table of Contents

- [HTTP in detail](#http-in-detail)
        - [Learn about how to request content from a web server using the HTTP protocol](#learn-about-how-to-request-content-from-a-web-server-using-the-http-protocol)
        - [If you want to check out the room click here](#if-you-want-to-check-out-the-room-click-here)
    - [Table of Contents](#table-of-contents)
- [Task 1 What is HTTP(S)?](#task-1-what-is-https)
    - [What does HTTP stand for?](#what-does-http-stand-for)
    - [What does the S in HTTPS stand for?](#what-does-the-s-in-https-stand-for)
    - [On the mock webpage on the right there is an issue, once you've found it, click on it. What is the challenge flag?](#on-the-mock-webpage-on-the-right-there-is-an-issue-once-youve-found-it-click-on-it-what-is-the-challenge-flag)
- [Task 2 Requests and Responses](#task-2-requests-and-responses)
    - [What HTTP protocol is being used in the above example?](#what-http-protocol-is-being-used-in-the-above-example)
    - [What response header tells the browser how much data to expect?](#what-response-header-tells-the-browser-how-much-data-to-expect)
- [Task 3 HTTP Methods](#task-3-http-methods)
    - [What method would be used to create a new user account?](#what-method-would-be-used-to-create-a-new-user-account)
    - [What method would be used to update your email address?](#what-method-would-be-used-to-update-your-email-address)
    - [What method would be used to remove a picture you've uploaded to your account?](#what-method-would-be-used-to-remove-a-picture-youve-uploaded-to-your-account)
    - [What method would be used to view a news article?](#what-method-would-be-used-to-view-a-news-article)
- [Task 4 HTTP Status Codes](#task-4-http-status-codes)
    - [What response code might you receive if you've created a new user or blog post article?](#what-response-code-might-you-receive-if-youve-created-a-new-user-or-blog-post-article)
    - [What response code might you receive if you've tried to access a page that doesn't exist?](#what-response-code-might-you-receive-if-youve-tried-to-access-a-page-that-doesnt-exist)
    - [What response code might you receive if the web server cannot access its database and the application crashes?](#what-response-code-might-you-receive-if-the-web-server-cannot-access-its-database-and-the-application-crashes)
    - [What response code might you receive if you try to edit your profile without logging in first?](#what-response-code-might-you-receive-if-you-try-to-edit-your-profile-without-logging-in-first)
- [Task 5 Headers](#task-5-headers)
    - [What header tells the web server what browser is being used?](#what-header-tells-the-web-server-what-browser-is-being-used)
    - [What header tells the browser what type of data is being returned?](#what-header-tells-the-browser-what-type-of-data-is-being-returned)
    - [What header tells the web server which website is being requested?](#what-header-tells-the-web-server-which-website-is-being-requested)
- [Task 6 Cookies](#task-6-cookies)
    - [Which header is used to save cookies to your computer?](#which-header-is-used-to-save-cookies-to-your-computer)
- [Task 7 Making Requests](#task-7-making-requests)
    - [Make a GET request to /room](#make-a-get-request-to-room)
    - [Make a GET request to /blog and using the gear icon set the id parameter to 1 in the URL field](#make-a-get-request-to-blog-and-using-the-gear-icon-set-the-id-parameter-to-1-in-the-url-field)
    - [Make a DELETE request to /user/1](#make-a-delete-request-to-user1)
    - [Make a PUT request to /user/2 with the username parameter set to admin](#make-a-put-request-to-user2-with-the-username-parameter-set-to-admin)
    - [POST the username of thm and a password of letmein to /login](#post-the-username-of-thm-and-a-password-of-letmein-to-login)

# Task 1 What is HTTP(S)?

### What does HTTP stand for?

    HyperText Transfer Protocol

### What does the S in HTTPS stand for?

    Secure

### On the mock webpage on the right there is an issue, once you've found it, click on it. What is the challenge flag?

    Can't be provided under THMs terms for submiting writeups in their rooms.

# Task 2 Requests and Responses

### What HTTP protocol is being used in the above example?

    HTTP/1.1

### What response header tells the browser how much data to expect?

    Content-Length

# Task 3 HTTP Methods

### What method would be used to create a new user account?

    POST

### What method would be used to update your email address?

    PUT

### What method would be used to remove a picture you've uploaded to your account?

    DELETE

### What method would be used to view a news article?

    GET

# Task 4 HTTP Status Codes

### What response code might you receive if you've created a new user or blog post article?

    201

### What response code might you receive if you've tried to access a page that doesn't exist?

    404

### What response code might you receive if the web server cannot access its database and the application crashes?

    503

### What response code might you receive if you try to edit your profile without logging in first?

    401

# Task 5 Headers

### What header tells the web server what browser is being used?

    User-Agent

### What header tells the browser what type of data is being returned?

    Content-Type

### What header tells the web server which website is being requested?

    Host

# Task 6 Cookies

### Which header is used to save cookies to your computer?

    Set-Cookie

# Task 7 Making Requests

### Make a GET request to /room

    Can't be provided under THMs terms for submiting writeups in their rooms.

### Make a GET request to /blog and using the gear icon set the id parameter to 1 in the URL field

    Can't be provided under THMs terms for submiting writeups in their rooms.

### Make a DELETE request to /user/1

    Can't be provided under THMs terms for submiting writeups in their rooms.

### Make a PUT request to /user/2 with the username parameter set to admin

    Can't be provided under THMs terms for submiting writeups in their rooms.

### POST the username of thm and a password of letmein to /login

    Can't be provided under THMs terms for submiting writeups in their rooms.
