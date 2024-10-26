# TryHackMe Room Name: Brains

![[Pasted image 20241026191605.png]]
 Room Link: https://tryhackme.com/r/room/brains 
# Red: Exploit the Server

**Goal: Get the contents of the User Flag**

Attack Path:
1. We found ports 22, 80, 50000 open on the target
2. Ports 22 and 80 lead to nowhere
3. Port 50000 has an application called TeamCity running on it
4. We did some research and found this version of TeamCity is vulnerable to an authentication bypass (CVE-2024-27198)
5. Referencing this [Rapid7 blog](https://www.rapid7.com/blog/post/2024/03/04/etr-cve-2024-27198-and-cve-2024-27199-jetbrains-teamcity-multiple-authentication-bypass-vulnerabilities-fixed/) we use metasploit to gain a shell on the target
6. We can find the user flag through the shell!

# Blue: Let's Investigate

**Goal: Identify the attacker's footprints in post-exploitation stage**

We are provided with a splunk instance along with credentials on the exploited machine. Using splunk we need to answer the following questions:
1. What is the name of the backdoor user which was created on the server after exploitation?  
2. What is the name of the malicious-looking package installed on the server?  
3. What is the name of the plugin installed on the server after successful exploitation?

To do this we will use the "Search & Reporting" feature of Splunk
## Backdoor User
Since we're looking for users, we will search the auth.log logs in `/var/log/auth.log`

## Malicious Package installed
Installed packages are generally logged at `/var/log/dpkg.log`, so that's where we look. 
❗We'll make sure to look for packages installed around the same time frame as the backdoored user so that it's easier to find the malicious package.

## Plugin Installed on Server
We simply searched plugins in splunk. 
Alternatively, we can search `TeamCity` logs