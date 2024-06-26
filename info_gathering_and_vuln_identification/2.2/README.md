## 2.2 Given a scenario, perform a vulnerability scan.
* Credentialed vs. non-credentialed
Providing administrative credentials to a system allows vulnerability scanners to authenticate and provide a much more comprehensive look at the target system.
* Types of scans
  * Discovery scans are generally very fast and high level. An example of a discovery scan would be a ping scan, which only checks for systems that reply to pings. The following example shows a ping scan. A discovery scan against a single target may include scanning for open ports, but for subnets you may want to tread lightly to avoid setting off any IDS systems.
	* nmap -sn xxx.xxx.xxx.xxx (this disables port scanning) 
  * Full scans may take quite some time, and are typically performed with credentials. Common vulnerability scanners include Tenable Nessus, Tripwire, and OpenVAS (open source).
  * Stealth scans are capable of evading some firewalls and IDS systems. One technique is to perform a TCS syn scan. It scans by initiating TCP connections but never completes the 3 way handshake. It sends syn packets, and if it receives an ack, the target system/port must be listening. The scan never sends the final ack.
	* nmap -sS xxx.xxx.xxx.xxx
  * Compliance scans are those which are necessary for companies to ensure companies are keeping with the standards set by governing bodies. The most common compliance scans are those for PCI DSS.
* Container security is a newer challenge. Fortunately there are several commercial tools available which are capable of scanning container images are finding vulnerabilities.
* Application scan
  * Dynamic analysis is performed through automated programs such as scanners and pentesting against live applications. 
  * Static analysis is performed by analyzing the code base. There are scanners which will analyze for code flaws, back doors, and other malicious indicators.
* Considerations of vulnerability scanning
  * Time to run scans
  * Protocols used
  * Network topology
  * Bandwidth limitations
  * Query throttling
  * Fragile systems/non-traditional assets
