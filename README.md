# HackerGPT Lite Docs

<a href="https://hackergpt.app/" target="_blank">HackerGPT Lite</a> is a publicly available web OSINT and Discovery tool. Its free to use for first N interactions. You can start using it with existing Google account.

Watch it perform SQL injection on OWASP Juice Shop:

[![HackerGPT Lite](https://img.shields.io/badge/HackerGPT-Lite-red)](https://hackergpt.app)


Sample Prompt:

```
check hackergpt.app
```
<video controls src="https://hackergpt.s3.us-east-1.amazonaws.com/assets/videos/browser_demo.mp4" title="HackerGPT Lite" width="1000" height="700" controls></video>

## Scanning

You can scan public targets using HackerGPT Lite, there are 4 types of scans you can perform:

1. Service Discovery
2. SYN Scan
3. TCP Scan
4. OS and Version detection

Sample Prompt:

```
Perform a service discovery scan on juice-shop.hackergpt.app
```

## SSL Scan

This tool will tell you versions of TLS/SSL the target site uses and if its vulnerable to heartbleed or other TLS-related vulnerabilities.

Sample Prompt:

```
Perform SSL Scan on juice-shop.hackergpt.app
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
perform a service discovery scan and find associated CVEs on juice-shop.hackergpt.app
```
2. After vulnerabilities are found prompt it with finding an exploit code:

```
find exploit script
```

## Onion Links Analysis

Scrapes and analyzes a list of onion links via the Tor proxy so you don't have to access them directly by yourself.

Sample Prompt:
```
analyze http://exampleonion.onion
```

## Browser

Navigates to the URL of your choice, gathers network logs

Sample Prompt:
```
open browser at https://juice-shop.hackergpt.app
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
