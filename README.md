# Project 8 - Pentesting Live Targets

Time spent: **X** hours spent in total

> Objective: Identify vulnerabilities in three different versions of the Globitek website: blue, green, and red.

The six possible exploits are:
* Username Enumeration
* Insecure Direct Object Reference (IDOR)
* SQL Injection (SQLi)
* Cross-Site Scripting (XSS)
* Cross-Site Request Forgery (CSRF)
* Session Hijacking/Fixation

Each version of the site has been given two of the six vulnerabilities. (In other words, all six of the exploits should be assignable to one of the sites.)

## Blue

Vulnerability #1: SQL Injection

![](gif/SQLI.gif)

Vulnerability #2: __________________


## Green

Vulnerability #1: Username Enumeration

![](gif/username_enumeration.gif)

Vulnerability #2: XSS

![](gif/XSS.gif)

## Red

Vulnerability #1: IDOR

![](gif/IDOR.gif)


Vulnerability #2: __________________


## Notes

Username Enumeration:
It took me a long while to find the failed/failure change of class in the DOM.  I was looking for a message of sorts instead of such a subtle change.  I also wasn't sure which form I was supposed to look at.

IDOR:
That one was a bit more straight forward once I got into the swing of things, I was pretty sure that it had to do with user ids.

SQLI:
I tried all the forms to no avail, although sometimes I would get a blank page with a bad request notification giving me a false positive on the blue and green site.  I figured it was a bug since I couldn't reliably reproduce the error.

![](png/error.png)

XSS:
That one was straight forward, it felt intuitive that the best place to inject was in the contact form.  Although I did encounter the error from above again.  It seems that when quickly and consecutively doing the same action on the 3 different sites, the third request will fail.




