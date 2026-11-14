# Mission 7: How Computers Communicate

## 1. Task / Objective

The objective of this mission was to understand basic networking concepts, observe network connectivity and DNS lookup using Terminal, and explain what happens when a website is opened in a browser.

## 2. Work Completed

### Task 7.1: Network Concepts

| Concept | Explanation | Example |
|---|---|---|
| LAN (Local Area Network) | A network covering a small geographical area. | Home Wi-Fi or a computer laboratory. |
| MAN (Metropolitan Area Network) | A network covering a city or a large campus area. | A network connecting multiple offices across a city. |
| WAN (Wide Area Network) | A network covering large geographical areas. | The Internet. |
| DNS (Domain Name System) | Translates human-readable domain names into IP addresses. | Translating `example.com` into an IP address. |
| Router | Connects networks and forwards data between them. | A home Wi-Fi router. |
| Protocol | A set of rules that devices follow to communicate. | HTTP, HTTPS and TCP/IP. |
| Packet Switching | Divides data into smaller packets that travel through a network and are reassembled at the destination. | Loading a webpage over the Internet. |
| Client-Server | A client requests a service, and a server provides it. | A browser requesting a webpage from a web server. |

### Task 7.2: Observing Network Information

**1. Connectivity test using ping**

Command used:

```bash
ping -c 4 example.com
```

Observed result:

- 4 packets transmitted.
- 4 packets received.
- 0% packet loss.
- Minimum round-trip time: 100.968 ms.
- Average round-trip time: 188.279 ms.
- Maximum round-trip time: 286.296 ms.

This showed that my computer could successfully reach the example.com network destination and receive replies.

**2. DNS lookup using nslookup**

Command used:

```bash
nslookup example.com
```

Observed result:

- The DNS lookup successfully resolved `example.com`.
- It returned two IPv4 addresses.
- The DNS resolver used by my computer was displayed in the output. Its address has been omitted for privacy.

This demonstrated how DNS translates a domain name into network addresses that computers can use.

**Questions and Answers**

**What does a connectivity test help check?**

A connectivity test helps determine whether a computer can reach another network destination. It can also provide information about response time and packet loss.

**What does a DNS lookup display?**

A DNS lookup displays information about the DNS resolver and the IP addresses associated with a domain name.

**What is the role of DNS when entering a website name in a browser?**

DNS translates the human-readable website name into an IP address so the browser can locate the appropriate server.

### Task 7.3: What Happens When You Open a Website?

When a user enters a website address such as `https://www.example.com` into a browser, the following steps take place:

1. **User enters a URL:** The user types a website address into the browser. The browser acts as the client.
2. **DNS lookup:** The browser or operating system obtains the IP address associated with the domain name using DNS.
3. **Connection establishment:** The device establishes a connection with the web server. For HTTPS, TLS provides secure communication.
4. **Request sent:** The browser sends an HTTP request to the web server.
5. **Data travels through the network:** Routers forward the data across networks. Data may be divided into smaller packets during transmission.
6. **Server responds:** The web server processes the request and sends an HTTP response containing the requested website content.
7. **Website displayed:** The browser processes the response, loads the required resources and displays the webpage to the user.

## 3. Commands / Tools Used

| Command / Tool | Purpose |
|---|---|
| `ping -c 4 example.com` | Checks connectivity by sending four network packets and measuring replies. |
| `nslookup example.com` | Performs a DNS lookup to find addresses associated with a domain. |
| Terminal | Used to execute networking commands. |
| Web browser | Used to understand the client-server communication process. |

## 4. My Understanding

Through this mission, I understood how computers communicate over networks and how different networking concepts work together.

I learned the differences between LAN, MAN and WAN, and understood how DNS helps computers locate websites using domain names. I also learned the roles of routers, protocols, packet switching and client-server architecture.

The practical exercises helped me understand how to check network connectivity using `ping` and how to find domain-related IP addresses using `nslookup`.

I also understood the sequence of events that takes place when a browser requests and displays a website.

## 5. Difficulties Faced

Initially, understanding the differences between LAN, MAN and WAN and the roles of DNS, routers and protocols required some effort.

I also needed to understand the information displayed by the `ping` and `nslookup` commands.

## 6. How I Resolved Them

I studied each networking concept with practical examples and understood how they are used in everyday communication.

I ran the networking commands in Terminal and examined their outputs. This helped me understand packet transmission, response time, packet loss and DNS resolution.

## 7. Evidence / Files

- `mission-07-networking/README.md` – Contains networking concepts, practical observations and the website communication process.
- Evidence of `ping` and `nslookup` command execution was observed in Terminal.

Personal network details, including the DNS resolver address, have been excluded for privacy.

## 8. Commit Details

Commit message: `Explain networking concepts and website communication`

## 9. Final Status

Mission 7 completed successfully. I explored basic networking concepts, tested network connectivity, performed a DNS lookup and documented the process of opening a website.