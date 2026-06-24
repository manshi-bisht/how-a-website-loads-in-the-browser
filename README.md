# Day 2 – What Happens When You Open a Website

Website tested: https://shorterloop.com

## DNS Lookup

Command used:

```bash
nslookup shorterloop.com
```

Output:

```text
Name:    shorterloop.com
Address: 76.76.21.21
```

## Network Requests

> Replace the sample details below with the exact requests shown in your Chrome Network tab.

### Request 1
- URL: https://shorterloop.com/
- Method: GET
- Status Code: 200 OK
- Type: document (HTML)
- Header: content-type: text/html

### Request 2
- URL: CSS file from Network tab
- Method: GET
- Status Code: 200 OK
- Type: stylesheet
- Header: content-type: text/css

### Request 3
- URL: JavaScript file from Network tab
- Method: GET
- Status Code: 200 OK
- Type: script
- Header: content-type: application/javascript

### Request 4
- URL: Image file from Network tab
- Method: GET
- Status Code: 200 OK
- Type: image
- Header: content-type: image/webp

### Request 5
- URL: Another request from Network tab
- Method: GET
- Status Code: 200 OK
- Type: fetch / xhr / font / script
- Header: Copy one response header from Chrome DevTools

## What I Learned

When I type a website address, DNS converts the domain name into an IP address. The browser then connects to the server using TCP, creates a secure connection using TLS, sends an HTTP request, receives files such as HTML, CSS, JavaScript, and images, and finally displays the webpage.
