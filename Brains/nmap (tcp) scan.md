```


# Nmap 7.94SVN scan initiated Sat Oct 26 17:02:44 2024 as: nmap -sC -sV -O -T5 -o full_tcpscan 10.10.240.146
Warning: 10.10.240.146 giving up on port because retransmission cap hit (2).
Nmap scan report for 10.10.240.146
Host is up (0.11s latency).
Not shown: 745 closed tcp ports (reset), 252 filtered tcp ports (no-response)
PORT      STATE SERVICE  VERSION
22/tcp    open  ssh      OpenSSH 8.2p1 Ubuntu 4ubuntu0.11 (Ubuntu Linux; protocol 2.0)
| ssh-hostkey: 
|   3072 a8:06:7e:c4:5a:8a:ea:61:68:16:d5:ab:f3:f9:ed:d2 (RSA)
|   256 a9:23:4c:49:11:62:f6:b8:aa:e9:5d:e4:c9:8e:5b:8c (ECDSA)
|_  256 9d:82:e4:90:bf:54:f7:9f:60:9b:1e:c2:f2:de:77:11 (ED25519)
80/tcp    open  http     Apache httpd 2.4.41 ((Ubuntu))
|_http-server-header: Apache/2.4.41 (Ubuntu)
|_http-title: Maintenance
50000/tcp open  ibm-db2?
| fingerprint-strings: 
|   drda, ibm-db2, ibm-db2-das: 
|     HTTP/1.1 400 
|     Content-Type: text/html;charset=utf-8
|     Content-Language: en
|     Content-Length: 435
|     Date: Sat, 26 Oct 2024 21:03:26 GMT
|     Connection: close
|     <!doctype html><html lang="en"><head><title>HTTP Status 400 
|     Request</title><style type="text/css">body {font-family:Tahoma,Arial,sans-serif;} h1, h2, h3, b {color:white;background-color:#525D76;} h1 {font-size:22px;} h2 {font-size:16px;} h3 {font-size:14px;} p {font-size:12px;} a {color:black;} .line {height:1px;background-color:#525D76;border:none;}</style></head><body><h1>HTTP Status 400 
|_    Request</h1></body></html>
1 service unrecognized despite returning data. If you know the service/version, please submit the following fingerprint at https://nmap.org/cgi-bin/submit.cgi?new-service :
SF-Port50000-TCP:V=7.94SVN%I=7%D=10/26%Time=671D591F%P=x86_64-pc-linux-gnu
SF:%r(ibm-db2-das,24E,"HTTP/1\.1\x20400\x20\r\nContent-Type:\x20text/html;
SF:charset=utf-8\r\nContent-Language:\x20en\r\nContent-Length:\x20435\r\nD
SF:ate:\x20Sat,\x2026\x20Oct\x202024\x2021:03:26\x20GMT\r\nConnection:\x20
SF:close\r\n\r\n<!doctype\x20html><html\x20lang=\"en\"><head><title>HTTP\x
SF:20Status\x20400\x20\xe2\x80\x93\x20Bad\x20Request</title><style\x20type
SF:=\"text/css\">body\x20{font-family:Tahoma,Arial,sans-serif;}\x20h1,\x20
SF:h2,\x20h3,\x20b\x20{color:white;background-color:#525D76;}\x20h1\x20{fo
SF:nt-size:22px;}\x20h2\x20{font-size:16px;}\x20h3\x20{font-size:14px;}\x2
SF:0p\x20{font-size:12px;}\x20a\x20{color:black;}\x20\.line\x20{height:1px
SF:;background-color:#525D76;border:none;}</style></head><body><h1>HTTP\x2
SF:0Status\x20400\x20\xe2\x80\x93\x20Bad\x20Request</h1></body></html>")%r
SF:(ibm-db2,24E,"HTTP/1\.1\x20400\x20\r\nContent-Type:\x20text/html;charse
SF:t=utf-8\r\nContent-Language:\x20en\r\nContent-Length:\x20435\r\nDate:\x
SF:20Sat,\x2026\x20Oct\x202024\x2021:03:26\x20GMT\r\nConnection:\x20close\
SF:r\n\r\n<!doctype\x20html><html\x20lang=\"en\"><head><title>HTTP\x20Stat
SF:us\x20400\x20\xe2\x80\x93\x20Bad\x20Request</title><style\x20type=\"tex
SF:t/css\">body\x20{font-family:Tahoma,Arial,sans-serif;}\x20h1,\x20h2,\x2
SF:0h3,\x20b\x20{color:white;background-color:#525D76;}\x20h1\x20{font-siz
SF:e:22px;}\x20h2\x20{font-size:16px;}\x20h3\x20{font-size:14px;}\x20p\x20
SF:{font-size:12px;}\x20a\x20{color:black;}\x20\.line\x20{height:1px;backg
SF:round-color:#525D76;border:none;}</style></head><body><h1>HTTP\x20Statu
SF:s\x20400\x20\xe2\x80\x93\x20Bad\x20Request</h1></body></html>")%r(drda,
SF:24E,"HTTP/1\.1\x20400\x20\r\nContent-Type:\x20text/html;charset=utf-8\r
SF:\nContent-Language:\x20en\r\nContent-Length:\x20435\r\nDate:\x20Sat,\x2
SF:026\x20Oct\x202024\x2021:03:26\x20GMT\r\nConnection:\x20close\r\n\r\n<!
SF:doctype\x20html><html\x20lang=\"en\"><head><title>HTTP\x20Status\x20400
SF:\x20\xe2\x80\x93\x20Bad\x20Request</title><style\x20type=\"text/css\">b
SF:ody\x20{font-family:Tahoma,Arial,sans-serif;}\x20h1,\x20h2,\x20h3,\x20b
SF:\x20{color:white;background-color:#525D76;}\x20h1\x20{font-size:22px;}\
SF:x20h2\x20{font-size:16px;}\x20h3\x20{font-size:14px;}\x20p\x20{font-siz
SF:e:12px;}\x20a\x20{color:black;}\x20\.line\x20{height:1px;background-col
SF:or:#525D76;border:none;}</style></head><body><h1>HTTP\x20Status\x20400\
SF:x20\xe2\x80\x93\x20Bad\x20Request</h1></body></html>");
Device type: WAP
Running: Actiontec embedded, Linux
OS CPE: cpe:/h:actiontec:mi424wr-gen3i cpe:/o:linux:linux_kernel
OS details: Actiontec MI424WR-GEN3I WAP
Service Info: OS: Linux; CPE: cpe:/o:linux:linux_kernel

OS and Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
# Nmap done at Sat Oct 26 17:03:53 2024 -- 1 IP address (1 host up) scanned in 68.97 seconds

```


# 50000
```
nmap -p 50000 brains.thm -sC -sV -T5

Starting Nmap 7.94SVN ( https://nmap.org ) at 2024-10-26 17:45 EDT
Nmap scan report for brains.thm (10.10.240.146)
Host is up (0.11s latency).

PORT      STATE SERVICE  VERSION
50000/tcp open  ibm-db2?
| fingerprint-strings: 
|   GetRequest: 
|     HTTP/1.1 401 
|     TeamCity-Node-Id: MAIN_SERVER
|     WWW-Authenticate: Basic realm="TeamCity"
|     WWW-Authenticate: Bearer realm="TeamCity"
|     Cache-Control: no-store
|     Content-Type: text/plain;charset=UTF-8
|     Date: Sat, 26 Oct 2024 21:45:30 GMT
|     Connection: close
|     Authentication required
|     login manually go to "/login.html" page
|   drda: 
|     HTTP/1.1 400 
|     Content-Type: text/html;charset=utf-8
|     Content-Language: en
|     Content-Length: 435
|     Date: Sat, 26 Oct 2024 21:45:35 GMT
|     Connection: close
|     <!doctype html><html lang="en"><head><title>HTTP Status 400 
|     Request</title><style type="text/css">body {font-family:Tahoma,Arial,sans-serif;} h1, h2, h3, b {color:white;background-color:#525D76;} h1 {font-size:22px;} h2 {font-size:16px;} h3 {font-size:14px;} p {font-size:12px;} a {color:black;} .line {height:1px;background-color:#525D76;border:none;}</style></head><body><h1>HTTP Status 400 
|     Request</h1></body></html>
|   ibm-db2: 
|     HTTP/1.1 400 
|     Content-Type: text/html;charset=utf-8
|     Content-Language: en
|     Content-Length: 435
|     Date: Sat, 26 Oct 2024 21:45:33 GMT
|     Connection: close
|     <!doctype html><html lang="en"><head><title>HTTP Status 400 
|     Request</title><style type="text/css">body {font-family:Tahoma,Arial,sans-serif;} h1, h2, h3, b {color:white;background-color:#525D76;} h1 {font-size:22px;} h2 {font-size:16px;} h3 {font-size:14px;} p {font-size:12px;} a {color:black;} .line {height:1px;background-color:#525D76;border:none;}</style></head><body><h1>HTTP Status 400 
|     Request</h1></body></html>
|   ibm-db2-das: 
|     HTTP/1.1 400 
|     Content-Type: text/html;charset=utf-8
|     Content-Language: en
|     Content-Length: 435
|     Date: Sat, 26 Oct 2024 21:45:30 GMT
|     Connection: close
|     <!doctype html><html lang="en"><head><title>HTTP Status 400 
|     Request</title><style type="text/css">body {font-family:Tahoma,Arial,sans-serif;} h1, h2, h3, b {color:white;background-color:#525D76;} h1 {font-size:22px;} h2 {font-size:16px;} h3 {font-size:14px;} p {font-size:12px;} a {color:black;} .line {height:1px;background-color:#525D76;border:none;}</style></head><body><h1>HTTP Status 400 
|_    Request</h1></body></html>
1 service unrecognized despite returning data. If you know the service/version, please submit the following fingerprint at https://nmap.org/cgi-bin/submit.cgi?new-service :
SF-Port50000-TCP:V=7.94SVN%I=7%D=10/26%Time=671D62FB%P=x86_64-pc-linux-gnu
SF:%r(GetRequest,140,"HTTP/1\.1\x20401\x20\r\nTeamCity-Node-Id:\x20MAIN_SE
SF:RVER\r\nWWW-Authenticate:\x20Basic\x20realm=\"TeamCity\"\r\nWWW-Authent
SF:icate:\x20Bearer\x20realm=\"TeamCity\"\r\nCache-Control:\x20no-store\r\
SF:nContent-Type:\x20text/plain;charset=UTF-8\r\nDate:\x20Sat,\x2026\x20Oc
SF:t\x202024\x2021:45:30\x20GMT\r\nConnection:\x20close\r\n\r\nAuthenticat
SF:ion\x20required\nTo\x20login\x20manually\x20go\x20to\x20\"/login\.html\
SF:"\x20page")%r(ibm-db2-das,24E,"HTTP/1\.1\x20400\x20\r\nContent-Type:\x2
SF:0text/html;charset=utf-8\r\nContent-Language:\x20en\r\nContent-Length:\
SF:x20435\r\nDate:\x20Sat,\x2026\x20Oct\x202024\x2021:45:30\x20GMT\r\nConn
SF:ection:\x20close\r\n\r\n<!doctype\x20html><html\x20lang=\"en\"><head><t
SF:itle>HTTP\x20Status\x20400\x20\xe2\x80\x93\x20Bad\x20Request</title><st
SF:yle\x20type=\"text/css\">body\x20{font-family:Tahoma,Arial,sans-serif;}
SF:\x20h1,\x20h2,\x20h3,\x20b\x20{color:white;background-color:#525D76;}\x
SF:20h1\x20{font-size:22px;}\x20h2\x20{font-size:16px;}\x20h3\x20{font-siz
SF:e:14px;}\x20p\x20{font-size:12px;}\x20a\x20{color:black;}\x20\.line\x20
SF:{height:1px;background-color:#525D76;border:none;}</style></head><body>
SF:<h1>HTTP\x20Status\x20400\x20\xe2\x80\x93\x20Bad\x20Request</h1></body>
SF:</html>")%r(ibm-db2,24E,"HTTP/1\.1\x20400\x20\r\nContent-Type:\x20text/
SF:html;charset=utf-8\r\nContent-Language:\x20en\r\nContent-Length:\x20435
SF:\r\nDate:\x20Sat,\x2026\x20Oct\x202024\x2021:45:33\x20GMT\r\nConnection
SF::\x20close\r\n\r\n<!doctype\x20html><html\x20lang=\"en\"><head><title>H
SF:TTP\x20Status\x20400\x20\xe2\x80\x93\x20Bad\x20Request</title><style\x2
SF:0type=\"text/css\">body\x20{font-family:Tahoma,Arial,sans-serif;}\x20h1
SF:,\x20h2,\x20h3,\x20b\x20{color:white;background-color:#525D76;}\x20h1\x
SF:20{font-size:22px;}\x20h2\x20{font-size:16px;}\x20h3\x20{font-size:14px
SF:;}\x20p\x20{font-size:12px;}\x20a\x20{color:black;}\x20\.line\x20{heigh
SF:t:1px;background-color:#525D76;border:none;}</style></head><body><h1>HT
SF:TP\x20Status\x20400\x20\xe2\x80\x93\x20Bad\x20Request</h1></body></html
SF:>")%r(drda,24E,"HTTP/1\.1\x20400\x20\r\nContent-Type:\x20text/html;char
SF:set=utf-8\r\nContent-Language:\x20en\r\nContent-Length:\x20435\r\nDate:
SF:\x20Sat,\x2026\x20Oct\x202024\x2021:45:35\x20GMT\r\nConnection:\x20clos
SF:e\r\n\r\n<!doctype\x20html><html\x20lang=\"en\"><head><title>HTTP\x20St
SF:atus\x20400\x20\xe2\x80\x93\x20Bad\x20Request</title><style\x20type=\"t
SF:ext/css\">body\x20{font-family:Tahoma,Arial,sans-serif;}\x20h1,\x20h2,\
SF:x20h3,\x20b\x20{color:white;background-color:#525D76;}\x20h1\x20{font-s
SF:ize:22px;}\x20h2\x20{font-size:16px;}\x20h3\x20{font-size:14px;}\x20p\x
SF:20{font-size:12px;}\x20a\x20{color:black;}\x20\.line\x20{height:1px;bac
SF:kground-color:#525D76;border:none;}</style></head><body><h1>HTTP\x20Sta
SF:tus\x20400\x20\xe2\x80\x93\x20Bad\x20Request</h1></body></html>");

Service detection performed. Please report any incorrect results at https://nmap.org/submit/ .
Nmap done: 1 IP address (1 host up) scanned in 35.19 seconds

```