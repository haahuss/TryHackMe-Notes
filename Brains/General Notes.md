
# Red
## IP Address
10.10.240.146


nmap scan:
```
sudo nmap -sC -sV -O -T5 brains.thm -o full_tcpscan
```


no robots.txt
no login
no apache vuln

gobuster gave nothing
```
gobuster dir -u 10.10.240.146/ -w /usr/share/wordlists/dirb/big.txt -t 100 
```


port 80 gives nothing


## 50000

ibm-db2

attack path:

search teamcity  Version 2023.11.3 (build 147512) exploit

Reference
https://www.rapid7.com/blog/post/2024/03/04/etr-cve-2024-27198-and-cve-2024-27199-jetbrains-teamcity-multiple-authentication-bypass-vulnerabilities-fixed/

set options

get a shell

get the user flag!


# Blue

## IP address
10.10.131.2

## Splunk
10.10.131.2:8000

### creds
splunk
analyst123


