# Pen Testing Live Targets

Time spent: **X** hours spent in total

> Objective: Identify vulnerabilities in three different versions of the Globitek website: blue, green, and red.

The six possible exploits are:

* Username Enumeration
* Insecure Direct Object Reference (IDOR)
* SQL Injection (SQLi)
* Cross-Site Scripting (XSS)
* Cross-Site Request Forgery (CSRF)
* Session Hijacking/Fixation

Each color is vulnerable to only 2 of the 6 possible exploits. First discover which color has the specific vulnerability, then write a short description of how to exploit it, and finally demonstrate it using screenshots compiled into a GIF.

## Blue

Vulnerability #1: SQL Injecion (SQLi)

Description: The hacker visits the sales person 
Robert Hamilton ```/public/salesperson.php?id=4``` and injects this specific SQL into the URL
```/public/salesperson.php?id=%27or%201=1--%27``` The URL returns the sales person Daron Burke.

<img src="./blueexploit1.gif">

Vulnerability #2: Session Hijacking/Fixation

Description: The victim Logs in to the website as the administrator, The hacker captures the administrator's session ID and logins into the administrator's account with the stolen session ID.

<img src="./blueexploit2.gif">


## Green

Vulnerability #1: Username Enumeration

Description:
When a hacker enters a correct username, they inspect the element of the username and find the ```class=failure``` element. If the username does not exist in the website, then the inspect of the username will return ```class=failed```. For example, the pperson username exists in the website but the ppersons username does not exist.

<img src="./greenexploit1.gif">

Vulnerability #2: Cross-Site Scripting (XSS)

Description:
The hacker takes advantage of a cross-site scripting vulnerablility in the contact form.
When the administrator logs in, and visits the feedback page, they are attacked by a cross-site script.

<img src="./greenexploit2.gif">

## Red

Vulnerability #1: __________________

Description:

<img src="red-vuln1.gif">


## Notes

Describe any challenges encountered while doing the work

