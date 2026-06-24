# What Happens When You Open a Website

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

Observation:

```text
The DNS (Domain Name System) translated the domain name shorterloop.com into the IP address 76.76.21.21, allowing the browser
 to locate the web server.
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

When I type a website address into a browser, the DNS system first converts the domain name into an IP address. The browser then establishes a TCP connection with the server and creates a secure connection using TLS (Transport Layer Security). After the connection is established, the browser sends an HTTP request to the server. The server responds by sending files such as HTML, CSS, JavaScript, images, and other resources. The browser downloads these files, processes them, and renders the webpage on the screen.

## Result

Successfully observed the process of loading a website by performing a DNS lookup and analyzing network requests in Chrome DevTools. Learned how DNS resolution, TCP connection, TLS encryption, HTTP requests, and webpage resources work together to display a website.
