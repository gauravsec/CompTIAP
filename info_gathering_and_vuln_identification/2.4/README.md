# 2.4 Explain the process of leveraging information to prepare for exploitation.
## Map vulnerabilities to potential exploits
There are several ways you can map vulnerabilities to potential exploits. One way is to use nmap scripts, which need to be downloaded
* nmap --script nmap-vulners -sV xxx.xxx.xxx.xxx
* nmap --script vulscan -sV xxx.xxx.xxx.xxx
* searchsploit cve-xxxx-xxxx
# Prioritize activities in preparation for penetration test
## Describe common techniques to complete attack
* Cross-compiling code is a technique which will allow some Windows exploits to run on Linux (or vise-versa).
	* Common example is Mingw-w64
* Exploit modification is a technique where you will change the code for any number of reasons including customization and changing the footprint/hash to avoid detection.
* Exploit chaining is the process of using one exploit to compromise a system, and then using another exploit to gain access to another.
* Proof-of-concept development (exploit development) is the process of developing code to demonstrate discovered vulnerabilities.
* Social engineering is the art of exploiting the inherit trusting nature or using scare/urgent/deceptive tactics to exploit people.
* Credential brute forcing is the process of guessing passwords.
* Dictionary attacks are similar to brute forcing, but the passwords are based off of common dictionary words.
* Rainbow tables are files which contain known passwords and their hashes. This technique is used for offline cracking.
* Deception
