# Room: DNS In Detail

**Module:** Module 3 — How The Web Works
**Date completed:** June 26, 2026

## What this room covers

This rooms covers the topic of DNS and the hierarchy of domains (gTLD and ccTLD, second level domain and sub-domains ) and the constraints on them ( like the character limit and that you can't use any special character except for a hyphen ) and then type of DNS records ( A Records, AAAA Records, MX Records, TXT Records and CNAME etc ) and lastly we learn how a DNS request is made

## Key concepts learned

- Domain Name System (DNS) — it is a system that labels the IP Addresses of websites with proper names or domains so that you don't have to remember the numbers instead you can simply remember an easy domain name like YouTube.com etc
- Global Top Level Domain (gTLD) — These are the domains that are used globally and are used to represent the type of website for example .com is for commercial websites while .org and .gov are for organisations and government websites respectively
- Country Code Top Level Domain (ccTLD) — These are domains specific to a country and are used to tell the geographical location of a website like .co.uk for websites in UK and .pk for websites in Pakistan etc
- Second Level Domain — it is basically the name of the website or domain like in youtube.com - youtube is the Second level domain while .com is the TLD although it has some limits like the character limit is 63 characters and you can only use a-z, 0-9 and hyphen
- Sub-domains — these are domains that are used before the second level domain and separated using a period (.) and they have their own limits etc
- A Records — These are the most important type of record and they resolve to IPv4 addresses ( basically a label for the IPv4 addresses ) like let's say there is a IPv4 address: 142.163.631.4 and we attach it or label it with the domain name of example.com then this is an A Record
- AAAA Record — Same as above but just for IPv6 addresses
- CNAME Record — it is basically a way to label a domain name itself like an IP resolve to a domain and then that domain again resolves to another domain
- MX Records — These are the records for gmail servers basically and they can be useful to get information
- TXT Records — These are just text records that hold text like all the gmails that a company uses so that the users can know if an email sent to them is from the company or a spam etc
- DNS Request — So a DNS Request is made in 5 steps first of all you enter the domain you want to go like "chess.com" and in step no 1 your computer checks if the website DNS is stored locally ( it is done for sites you visit often like youtube.com etc ) and if it is then the request ends here and the DNS is given back as the output but if it is not present in the computer cache we move to Step 2 which is your computer making a request to a Recursive DNS Server and it is a server that holds all the recently searched up domains ( it includes all the popular and most searched up domains ) and it goes through them to see if the domain is there and if it is not then we move on to Step 3 and it is the Root DNS Servers they are like a detective that knows and scans through all the TLD's and point your to the one that you need for example in Chess.com it is .com so it will send you to the servers hosting all the .com domains and there it sends you to a authoritative server or a nameserver which is the Step 4 and they hold the data for a particular domain ( the domain you searched for i.e Chess.com ) and laslty at Step 5 they return the data back to you and you go to that particular domain ( if the status is 200 otherwise it shows that there is some problem )

## Tools/commands used

- `nslookup website.com` — It is a command used to make requests to website and return the output for example I ran it on youtube.com and got this data:

Server: 127.0.0.1
Address: 127.0.0.1#53

Non-authoritative answer:
Name: youtube.com
Address: 142.250.202.238
Name: youtube.com
Address: 2a00:1450:4018:812::200e

we got their IPv4 and IPv6 address which both point to the domain youtube.com although searching the IPv4 takes you to google.com because youtube is owned by them and because this is the common IPv4 for all google websites so each time we search up for YouTube google adds a secret link into the header as a result we end up on youtube.com

## Something that confused me at first

The domain records and the type of records confused me a lot like I still don't completely understand the concept because maybe i have never seen a MX record or a gmail server but I saw their video on the room and in that the person states that right now we just need to know about the A Records and that I understand quite good they resolve IPv4 into domains and the others will be touched upon later so right now i am not searching anything up because I think that my understanding right now is good enough but if I end up seeing any of these later I will learn them completely

Also the Recursive DNS Server and the authoritative server or the name server are words i am hearing for the first time I know that these are servers with information on them but still they are a bit confusing

## How this connects to real-world security

It is a real world concept of DNS and how they work and how requests are made and what are the components in the process and that means that you can exploit them as well I don't know how but since it is a process that means that you can enter into it and exploit it in this way it connects to real world security

## Next steps / what I want to explore more

I want to move on to the next room
