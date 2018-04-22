# Project 8 - Pentesting Live Targets

Time spent: **12-13** hours spent in total

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

Vulnerability #1: SQL Injection (SQLi)

the website is vulnerable to sqli attacks.  

Vulnerability #2: Session Hijacking/Fixation

if you are not a user and you just happen to get the session id of someone who is a user, you can change your session id and using "hacktools/change_session_id.php" you can get logged in from his profile

## Green

Vulnerability #1: Cross-Site Scripting (XSS)

a malicous user can use xss to send stuff

Vulnerability #2: Username Enumeration

the website reveals too much information. if you sign in from a user that is in the database "login was unsuccessful" returns in a bolded letters, but if you sign in to someone that isn't in the database "login was unsuccessful" comes back in regular text

## Red

Vulnerability #1: Insecure Direct Object Reference (IDOR)

if you change the id # to 10 or 11 you can access data that isn't supposed to be accessed by the public

Vulnerability #2: Cross-Site Request Forgery (CSRF)

When changing the value of csrd_token, we still can make a change. other colors retun some error message

## extra
#1. another xss vulnerability found on the green website. you can force someone to go to a malicous website if they click on the feedback button
#2. (another blue problem) Session Hijacking / Fixation - A new session ID is not regenerated when logging back in.


## Notes
not sure how to embed the gifs into the readme file but everything is named according to their file names
Describe any challenges encountered while doing the work
