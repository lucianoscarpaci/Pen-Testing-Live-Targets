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


## Green

Vulnerability #1: __________________

Description:

<img src="green-vuln1.gif">


## Red

Vulnerability #1: __________________

Description:

<img src="red-vuln1.gif">


## Notes

Describe any challenges encountered while doing the work

