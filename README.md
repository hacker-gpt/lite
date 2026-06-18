# HackerGPT Lite Docs

<a href="https://hackergpt.app/" target="_blank">HackerGPT Lite</a> is a publicly available web OSINT and CTF Solving tool. You can start using it with existing Google account.

[![HackerGPT Lite](https://img.shields.io/badge/HackerGPT-Lite-red)](https://hackergpt.app)

> 🚩 Want to see it solve full Capture-the-Flag challenges? Read the **[CTF Mode field guide](ctf/)** — a screenshot walkthrough of HackerGPT attacking a live OWASP Juice Shop target. (See [CTF Mode](#ctf-mode) below.)

Sample Prompt:

```
check cybergym.hackergpt.app
```

## Scanning

You can scan public targets using HackerGPT Lite, there are 4 types of scans you can perform:

1. Service Discovery
2. SYN Scan
3. TCP Scan
4. OS and Version detection

Sample Prompt:

```
Perform a service discovery scan on cybergym.hackergpt.app
```

## Web Fingerprinting

Identify the technologies, server software and versions running on a target web application — the first step before looking for known vulnerabilities.

Sample Prompts:

```
check cybergym.hackergpt.app
fingerprint hackergpt.app
```

## SSL Scan

This tool will tell you versions of TLS/SSL the target site uses and if its vulnerable to heartbleed or other TLS-related vulnerabilities.

Sample Prompt:

```
Perform SSL Scan on cybergym.hackergpt.app
```

## Dark Web Search

Searches dark web and presents you with screenshots of found `.onion` pages:

Sample Prompts:

```
Search Dark Web for HackerGPT
Search Dark Web for Ferdinand Data Breach
```

## Geo IP Location

Find coordinates of an IP address or a domain name.


Sample Prompt:

```
Find geo location of hackergpt.app
```

## WHOIS Search

Sample Prompt:

```
Find domain registration details for hackergpt.app
```

## Find subdomains

Sample Prompt:

```
Find subdomains for wikipedia.org
```
## VIN Lookup

```
Search VIN WP0CD2A80RK228485
Search VIN WP0CB2A87RK223547
```

## CVE Search

Sample Prompts:
```
Find all CVEs for OpenSSH version 9.1
Find all CVEs for Grafana 10.0
```

## Network Scan, CVE Search & Exploit code

1. Combine several tools to produce more meaningful results

Sample Prompt:
```
perform a service discovery scan and find associated CVEs on testphp.vulnweb.com
perform a service discovery scan and find associated CVEs on cybergym.hackergpt.app
```
2. After vulnerabilities are found prompt it with finding an exploit code:

```
find exploit script
```

## Browser

Navigates to the URL of your choice, gathers network logs

Sample Prompts:
```
open browser at https://cybergym.hackergpt.app
GO_TO_URL http://testphp.vulnweb.com/
```

## Image EXIF / Metadata Analysis

Extract EXIF metadata from an image URL — camera model, software, timestamps and GPS coordinates where present. Useful for verifying image authenticity and geolocating photos.

Sample Prompt:

```
extract exif data from https://hackergpt.s3.us-east-1.amazonaws.com/assets/sample.jpg
```

## Crypto Analysis Tools

HackerGPT Lite includes several new crypto analysis features. These tools let you analyze tokens and wallets across different blockchains (Ethereum, Bitcoin, Solana, BSC, POL, etc.) and also check on-chain data like transactions, security, and sanctions.

### 1. Token analysis 
Retrieves detailed token information including general info, platform details, and security analysis. 

Sample Prompts: 
```
check TRUMP token
give complete detail of BNB token
```
### 2. Ethereum wallet analysis 
Analyzes an Ethereum wallet by retrieving its ETH balance, transaction history, and other token holdings.

Sample Prompts: 
```
analyze wallet 0x21E71B5AbdAf8F6a197648FdeB62C8948EAa8F5F
check 0x1da5821544e25c636c1417ba96ade4cf6d2f9b5a
```

### 3. Bitcoin wallet analysis 
Analyzes a Bitcoin wallet by fetching its BTC balance, transaction history, and USD equivalents.

Sample Prompts: 
```
analyze Bitcoin wallet 3J98t1WpEZ73CNmQviecrnyiWrnqRhWNLy
give me recent transaction history of 3J98t1WpEZ73CNmQviecrnyiWrnqRhWNLy
```

### 4. Sanctioned address check
Checks if a cryptocurrency wallet address is sanctioned against global economic and trade embargo lists.

Sample Prompts: 
```
check if wallet address 0x1da5821544e25c636c1417ba96ade4cf6d2f9b5a is sanctioned
is this wallet safe to deal with? 0x1da5821544e25c636c1417ba96ade4cf6d2f9b5a
```


Premium Features
=======================================

Premium features are available for HackerGPT Lite Subscribers.

## CTF Mode

CTF Mode turns HackerGPT Lite into an autonomous web-exploitation agent. Give it a target URL and it fingerprints the app, maps the attack surface from the static frontend, then drives a real browser session to confirm and exploit vulnerabilities — SQL injection, broken access control (IDOR), XSS, sensitive-data exposure, layered-encoding challenges and more.

As it works it builds a live workspace alongside the chat:

- **Network** — the raw request/response log of everything the agent sends; any request can be promoted with **Save as Payload**.
- **Payloads** — a vault of saved exploit requests you can expand and **Replay** with one click.
- **API Map** — the target's backend API surface, auto-discovered from the crawl.
- **Memory** — a persistent scratchpad of findings, credentials and confirmed vulnerabilities that carries across turns.

📖 **[Read the full CTF Mode field guide &rarr;](ctf/)** — a step-by-step walkthrough, with screenshots, of HackerGPT solving challenges on a live OWASP Juice Shop target and using the Payloads, API Map, Memory and Network panels.

Sample Prompts:

```
Analyze https://cybergym.hackergpt.app and discover all the injection vulnerabilities
Solve the Login Admin challenge on cybergym.hackergpt.app
```

## Face Search

Reverse-search a face across the public web using a photo you upload or an Instagram handle, to help identify or attribute a person.

Sample Prompt:

```
face search insta: @stevecarell
```

You can also upload a photo and ask HackerGPT to find where that face appears online.

## Phone Lookup (US numbers only)

Look up phone owners and their registered address location

Sample Prompt:

```
check the phone number location: 646-450-2377
check the owner of this phone number: 646-450-2377
```

## Email book

Find confirmed emails addresses for a certain domain name

Sample Prompt:

```
find emails for android.com
```

## Leaks search

Find if a token/email/username is in recent leaks

Sample Prompts:

```
check daryanrayne@gmail.com
check schamimahmut@gmail.com
```

## Crypto analysis on Solana chain

Analyzes crypto wallets and tokens on SOL chain by fetching its total balance, individual token details, and associated risks (rug-pull probability).

Sample Prompts:

```
is TRUMP token a rugpull?
analyze wallet 7rE6Q4c89bPiTqHg5Q67CbfnbYc8g43G7tEX5ZRbp8GG
```
