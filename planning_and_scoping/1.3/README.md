# 1.3 Explain the importance of scoping an engagement properly.
## Types of assessment
### Goals/objectives-based
These type of assessments are targeting specific goals or objectives which a client is interested in testing. This may be something such as a new website/server, feature such as 2FA, or perhaps even targeting VIPs.
### Compliance-based
There are required tests which are generally on an annual basis in order to keep compliance with the standard. The most common standard a pentester will be called in for will be for PCI (Payment Card Industry) which dictates the minimum standards a company needs to adhere to for handling customer payment card data.
### Red team
A red team may be brought in to test the effectiveness of a companies blue team. This type of assessment is designed to test the blue teams ability to protect against an active attack.

## Special scoping considerations
### Premerger
Before 2 companies merge, it is not uncommon for the parent company to request a pentest of the company they are consuming. This is to ensure the company is not inheriting more risk than in intends to.
### Supply chain
A companies supply chain is often one of the greatest sources of threats. If a supplier has a weakness, they may pose a threat to the company. A pentest of the supplier may be ordered before any business agreements are made.

## Target selection
### Targets
Targets of a pentest may include nearly any part of a companies infrastructure including but not limited to:
* Websites
* Servers
* People
* Physical infrastructure (gates, doors)
* And possibly more

### Internal vs External
Understanding where your target is in relation to the company is important. If a target is considered internal, will you need to request access to it? Or is this server widely available from the internet? This distinction needs to be understood before a pentest begins.
### On-site vs. off-site
Datacenters today are trending more towards off-site as the cloud becomes more prevalent and cost effective for companies. However on-site datacenters are still very prevalent with many companies and those in the government sector.
### First-party vs. third-party hosted
First-party applications are those which are running on servers within the companies datacenters or cloud environments. Third-party hosted applications are those which reside in the providers datacenters or cloud environments.
### Physical
It's possible that a pentest may include an element of physical testing. This may involve physically attempting to enter a building or tampering with a device.
### Users
Users are often considered the weakest part of any cybersecurity program, so it makes sense that a company will want to test them and often. Testing may include phishing, vishing, or any other type of social engineering.
### SSIDs
A company Wi-Fi can prove to be a great entry point to their corporate network. These SSIDs should be limited to the walls of the company. An over extended Wi-Fi may give an attacker ample opportunity to brute force passwords.

Another consideration for SSIDs are the ability for an attacker to spoof the network SSID in an effort to trick a user and gather their logon credentials. (Evil Twin attack)
### Applications
Knowledge of various applications used by the company can give an attacker an edge. An attacker can research publicized bugs and exploits which the attacker could use to gain entry into the network.
### Considerations
Some considerations when selecting your target should include:
* Target criticality - if a server is critical to a business to function, perhaps it's not a good idea to attack it
* Time - if you are attacking a target at a busy time of day, and bringing it down may effect business, reconsider.
### White-listed vs. black-listed
If you are not given direct access clients network, make sure your external IP is not blacklisted. It is probably a good idea to have your IP whitelisted to ensure you are able to complete your full test.
### Security exceptions
Before performing any testing, especially against cloud assets, ensure the proper security exceptions are in place to protect you.
### IPS/WAF whitelist
Ensure the IP from which you are performing your testing is whitelisted wherever necessary including IPSs and WAFs
### NAC
Ensure you have all of the necessary network access controls necessary to perform your test.
### Certificate pinning
You may need to provide the company a copy of your public key in order for them to trust the traffic coming from your systems.
### Company’s policies
Ensure you are aware of any applicable company policies in place. You may find lots of information out in a companies own policies such as password requirements, which can potentially be used against them in an attack.

## Strategy
### Black box
The smallest amount of necessary knowledge is provided to the attacker. This provides the truest test of a companies security.
### White box
Any information needed including source code is provided to the attacker. This type of test often provides the highest amount of results.
### Gray box
A type of testing which is a blend of black and white testing.

## Risk acceptance
This is the amount of risk a company is willing to accept. Some companies are able and willing to accept some amount of risk on their network. Others, especially those in regulated industries, might have a low acceptance of risk.

## Tolerance to impact
Your pentest may negatively impact services. It is important to communicate this to your client, and to ensure you stay within their tolerance levels.

## Scheduling
Your timeline should be clearly spelled out in your SOW, and you should ensure you stick to it. If any changes are necessary, make sure this is communicated with your client.

## Scope creep
Scope creep is a factor in nearly every project. This 'extra' work needs to be managed to ensure a timely delivery of agreed upon deliverables. Any work not specifically called out in the SOW will need to be agreed upon by both parties before adding it.

## Threat actors
### Adversary tiers
#### APT
Advanced Persistent Threats are major hacking groups that are often well funded. They have the most advanced capabilities and will methodically perform attacks over the course of long periods of time.
#### Script kiddies
Attackers who are not after anything in particular. Often times attack for 'street cred'. They tend to run other peoples code with a lower understanding of how the code actually works.
#### Hacktivist
Attackers who intend to exploit a company due to political or moral reasons.
#### Insider threat
A very dangerous attacker. Someone who is close to the company, usually an employee, who often times has privileged access. They leverage their position to exploit the company.
### Capabilities
Understanding the capabilities of those threat actors who are most likely to attack your company is important when building your defenses.
### Intent
Understanding the intent of those threat actors who are most likely to attack your company is important as well. Are they trying to deface your websites or are they stealing company secrets?
### Threat models
Threat modeling is the process of identifying, enumerating, and prioritizing different attack chains which may be used against a line of business. This helps the business identify potential weak points that may have been missed.
