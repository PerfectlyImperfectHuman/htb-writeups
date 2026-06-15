# Room: Offensive Security Intro

**Module:** Module 1 — Introduction to Cybersecurity
**Date completed:** June 15, 2026

## What this room covers

It gives a brief introduction to Offensive Security ( where we hack/break into systems ) using a practical approach ( we hack a fake bank website ) and concludes by telling us about some of the career paths in Cyber Security

## Key concepts learned

- Concept 1 — Offensive security means hacking into systems like a real hacker to find loopholes and then fix them so that real hackers can't break into them
- Concept 2 - Careers include Penetration Tester, Red Teamer and Security Engineer

## Tools/commands used

- `gobuster -u http://fakebank.thm -w wordlist.txt dir` — it tells the app gobuster to go through the entire wordlist and try and check if a page exists for each word and return the results

## Something that confused me at first

This command didn't make sense: gobuster -u http://fakebank.thm -w wordlist.txt dir but I understand a few things you add -u before a url and -w to give the wordlist file, gobuster is the name of the application we are using to go through the word list ( it basically takes the url and add all the wordlist as pages at the end like /app etc ). One thing I find interesting is that we http here and not https

Just learned about http and https and https encrypts the data before sending it while http sends it as plain text so anyone can easily read it

## How this connects to real-world security

A hacker can get admin access if the admin page is not secured properly. It also teaches us why we should use https and not http especially for sites like banks that need to be secured completely

## Next steps / what I want to explore more

The practical was fun and I want to try something like that in real life like use gobuster command on a real website
