## 2.1 Given a scenario, conduct information gathering using appropriate techniques.
## Scanning
Scanning is the process of identifying network hosts and vulnerabilities. There are several different scanners available from vendors and open-source. Some popular choices include Nmap, Tenable, and OWASP Zap.
## Enumeration
Enumeration is the process of discovering information.
  * Hosts: Find live hosts using nmap:
    * nmap -sP xxx.xxx.xxx.xxx/xx (ping scan)
    * nmap -sT xxx.xxx.xxx.xxx/xx (tcp scan)
    * nmap -sU xxx.xxx.xxx.xxx/xx (udp scan)
    * nmap -sS xxx.xxx.xxx.xxx/xx (stealth syn scan)
    * nmap -Pn xxx.xxx.xxx.xxx/xx (no ping, skips the discovery stage which commonly fails in networks where ping is disabled)
    * nmap -sV xxx.xxx.xxx.xxx/xx (service/version detection)
    * nmap -sn xxx.xxx.xxx.xxx/xx (disable port scan, only pings)
  * Networks:
    * nbtscan xxx.xxx.xxx.xxx/xx (discover Windows/Samba servers on subnet)
    * enum4linux -a xxx.xxx.xxx.xxx/xx (find windows client domain/workgroup)
    nmap -p <port number> xxx.xxx.xxx.xxx/xx (find all hosts running a service)
  * Domains: Discover domains via DNS:
    * dnsrecon -d example.com -D /usr/share/wordlists/dnsmap.txt (brute force subdomains on example.com using a given wordlist)
    * dnsrecon -r xxx.xxx.xxx.xxx/xx (reverse lookup of a range)
    * dnsmap example.com (another option. can specify word file using the -w argument)
  * Users: These are for SMB, there are of course dozens of other services we could perform this against.
    * nmap --script=smb-enum-users xxx.xxx.xxx.xxx/xx
    * (Metasploit) use auxiliary/scanner/smb/smb_lookupsid
    For windows MS-RPC
    * rpcclient -U "" -N xxx.xxx.xxx.xxx enumdomusers (will enum all users on the system)
  * Groups
    * nmap --script=smb-enum-groups xxx.xxx.xxx.xxx
  * Network shares
    * smbmap -u username -p password -H xxx.xxx.xxx.xxx (shows available shares for the given credentials)
    * nmap --script=smb-enum-shares xxx.xxx.xxx.xxx
  * Web pages
    * nmap --script=http-enum example.com
    * nikto -host example.com
  * Applications
  * Services
    * nmap -sV xxx.xxx.xxx.xxx/xx
    * nmap --script=smb-enum-processes --script-args= smbusername=admin,smbpass=password
  * Tokens
  * Social networking sites
    * Recon-ng
* Packet crafting
  * netcat
  * hping
  * scapy
* Packet inspection
  * tcpdump
  * wireshark
* Fingerprinting is the ability to determine things such as OS by performing a simple scan. An example using nmap:
  * nmap -O xxx.xxx.xxx.xxx
* Cryptography is important to understand. There are several different types of cryptography including DES, AES, and RSA. DES and AES are known as single key or symmetric algorithms. RSA is known as public key encryption which requires both the sender and receiver have public and private keys.
  * Certificate inspection can be performed either in the browser, or by using nmap:
    * nmap --script=ssl-cert example.com

* Eavesdropping can be done over a number of different methods including:
  * RF communication monitoring
  * Sniffing
  * Wired
  * Wireless
* Decompilation/Decompiler takes compiled code and attempts to turn it back into source code. If an attacker is able to successfully decompile code, they may be able to discover vulnerabilities in the code.
* Debugging software monitors applications as they are actively running and may give an attacker insight into how the application runs and how it might be exploited.
* Open Source Intelligence Gathering
  * Sources of research
  * CERT - Computer Emergency Readiness Team: Research center
  * NIST - National Institute of Standards and Technology: Creates Standards
  * JPCERT - Japan Computer Emergency Readiness Team
  * CAPEC -  Common Attack Pattern Enumeration and Classification: Used to classify attack pattern's seen in the wild.
  * Full disclosure
  * CVE
  * CWE
