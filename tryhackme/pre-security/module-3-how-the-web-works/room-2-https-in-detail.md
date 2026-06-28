# Room: HTTPS In Detail

**Module:** Module 3 — How The Web Works
**Date completed:** June 27, 2026

## What this room covers

The room covers the topic of HTTP & HTTPS ( HyperText Transfer Protocol-Secure ) what it is and what is it used for and how we access the resources of a website using URL and the components of a URL, We also learn how to make a GET Request and also learn about the different HTTP Methods and Status codes and lastly we learn about headers and cookies.

## Key concepts learned

HTTP/HTTPS:

- HyperText Transfer Protocol (HTTP) — are a set of rules that are used to communicate with the web server it was invented by Tim Berner's-Lee and his collegues
- HyperText Transfer Protocol-Secure (HTTPS) — is an encrypted and secure version of HTTP so that no one can see the data being transfered and it also gives you assurances that you're talking to the correct web server and not something impersonating it.

URL:

- Uniform Resource Locator (URL) — is a way to access the resources of a webpage or web server it is basically the text we type into the browser search bar like https://youtube.com
- Scheme of a URL — it is basically the protocol that is used in a url like https, http and ftp
- Host — This is the domain name of the website you are trying to access like in https://youtube.com - youtube.com is the domain name
- Path — it is the path after the host for example in youtube.com/explore - /explore is the path
- User — Some website require you to login so you need to add your login credentials into the URL
- Port — It is the port being used to access the page like :8080 etc
- Query String — It is the additional information that can be added like when you search something on Youtube the URL includes your query that is the query string
- Fragment — it is used to take you to a certain part of the page example #services etc

HTTP METHODS:

- GET Request — It is used to get data from a web server. Example: Getting your score-card online
- POST Request — It is used to submit new data to a web server. Example: Filling up a form
- PUT Request — It is used to update the existing data on a web server. Example: Updating your password or phone number
- DELETE Request — It is used to delete records from a web server. Example: Deleting your social media account

I thought of all the examples for the request right at the moment from what i can understand so some maybe wrong...

STATUS CODES:

- 100-199 — means that the first part of the request is successfully submitted and you can send the rest of the request. They are not used now (are deprecated)
- 200-299 — The Request was SUCCESSFULL!
- 300-399 — These are used to redirect the user to another page or website
- 400-499 — There was some kind of error on the user's end
- 500-599 — There was some kind of error on the server's end

HEADER ( Additional information you can send to a web server while making requests )

- HOST — to tell a server which website you want to access ( because many times a server hosts many sites )
- User-Agent — used to tell the server about the browser and the version so it can send proper data back for the specific browser
- Content-Length — tells the server how much data to expect in the request (especially when sending a form)
- Accept-Encoding — tells the browser how to compress or encode the data
- Cookies — Data sent to help the server remember who you are on the next visits
  (From Server)
- Set-Cookie — Data to send back to the server each time you send a request
- Cache-Control — Tells the browser for how much time it should store the website url/data in the browser cache
- Content-Type — Tells the browser what type of content is being sent back ( HTML, CSS & JS etc)
- Content-Encoding — tells the browser how the data is compressed or encoded

## Tools/commands used

Example Request:

GET / HTTP/1.1

Host: tryhackme.com
User-Agent: Mozilla/5.0 Firefox/87.0
Referer: https://tryhackme.com/

Example Response:

HTTP/1.1 200 OK

Server: nginx/1.15.8
Date: Fri, 09 Apr 2021 13:34:03 GMT
Content-Type: text/html
Content-Length: 98

<html>
<head>
    <title>TryHackMe</title>
</head>
<body>
    Welcome To TryHackMe.com
</body>
</html>

## Something that confused me at first

Well there was a lot in this room and I think i will have to come back here 2-3 times before i understand everything but from all the above these things confused me:

1. The User part of the URL: I have never seen the login information in the url ever before so maybe because of that or maybe because once you login or signup the url changes so quickly that you can't notice anything

2. The PUT Method: At first it confused me like what does it mean by updating but after thinking of an example I understand it completely fine

3. 100-199 Status Codes: Never seen them being used before but since they are deprecated now so it is understandable

4. The Set-Cookie Header: I was confused on it for a while but now i understand it is basically the data of the cookies that is stored on the browser that we send back each time a request is made to the server since the server forgets everything after it is done with the request

5. The Command and Response above confused me at first but after going through it line by line and understanding what each line meant now I can understand it

## How this connects to real-world security

It connects to the real world because every concept talked about above is part of the real world security like HTTP/HTTPS, URL, Status Codes and Headers they are all used all the time when you use the browser and search for something

## Next steps / what I want to explore more

I want to understand these things on a deeper level in the future
