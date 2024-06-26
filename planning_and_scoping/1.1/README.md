# 1.1 Explain the importance of planning for an engagement.

## Understanding the target audience
The end product of any penetration test is a clear, precise, and detailed report of the findings. Any number of individuals may be interested in reading this report, and it's important to keep that in mind as it is written. A manager may only be interested in a high level overview, whereas technical details may be better left in an appendix for the technical audience who may be find value in them while addressing the findings.

## Rules of engagement
The rules of engagement, or ROE, is a document which clearly outlines how the penetration test will be conducted. This should be agreed upon with the client before any testing begins. Some of the directives that should be covered include:

#### 1. Type and Scope
##### Types
There are a few different types of penetration tests which all provide different data.
  * Black box testing: The tester is provided a minimum amount of information such as an IP or domain name, most similar to what an attacker would have available. This type of test provides the closest to being attacked from a real attacker, however it may miss vulnerabilities present at a deeper or on a broader level.
  * White box testing: The tester is provided as many details as possible. IP's, domains, source code, usernames, or anything else which may help aide in discovering vulnerabilities. This type of testing will discover the most number of vulnerabilities, however it may not be the best simulation of what an attacker may perform.
  * Grey box testing: A combination of black and white testing, some understanding of the system or application is provided.

##### Scope
The scope specifies exactly what is being tested. Items not specified in the scope should not be tested, especially if it's people! Scope may include:
* Network
* Applications
* Web
* Mobile
* Cloud
* Physical
* Social engineering

#### 2. Client Contact Details
You will want to have at least one primary point of contact with their preferred method of contact documented. It is recommended that multiple contacts are documented as well as a clear escalation path in the event it is needed.

#### 3. Client IT Team Notifications
Penetration testing can cause unpredictable results against targets. Services may go down, devices may slow to a crawl, databases may corrupt, or a slew of many other situations may occur which the clients IT team would need to be notified of immediately. The way in which you notify and escalate the situation with the client should be clearly documented.

#### 4. Sensitive Data Handling
Throughout the course of your penetration test, there is always a possibility of coming across sensitive information. Knowing how to handle this information is crucial, as improper handling of this data may leave you legally accountable. Sensitive data may include, but not limited to:

* Health data (HIPAA)
* Credit card data (PCI)
* Adult content
* Personally Identifiable Information (PII)
* Protected data (Classified, Intellectual Properties, ect)

If you happen across any of the above materials, you need to immediately escalate to the designated contact(s). In some cases, you will need to immediately contact law enforcement. Don't ever copy, take screenshots, or interact in any way with any sensitive content as you may become legally accountable.

#### 5. Status Meetings and Progress Reports

## Communication escalation path
Keeping in touch with your client on a regular basis is important and should be planned. At any point during the engagement you may need to bring attention to things such as a system that has been inadvertently taken down or a critical vulnerability that has been discovered which requires immediate attention. The escalation path for such an event should be clearly documented during the planning phase of the engagement. Each client may have a different strategy. Some will have several contacts, while others may prefer to have one person who will serve as the main point of contact.

## Resources and requirements
* Confidentiality of findings - Ensure any findings during your engagement are kept confidential to avoid risking damage (reputation, data loss, exposure) to your client or yourself.
* Known vs. Unknown

## Impact analysis and remediation timelines
A key process to the requirements management process is the Impact Analysis (IA).
It is a formal approach to determine if something is or isn't necessary. It allows you to focus on some unexpected or negative side effects of performing an action.

## Technical Constraints and Organizational Budget
The organizational budget simply determines whether or not the budget exists to pay for a pentest.

Technical constraints are challenges the organization may have that could have negative effects when pentested. Examples may include legacy systems which may go down during vulnerability scans.

## Disclaimers
### Point-in-time-assessment
Applications and infrastructure are an ever evolving ecosystem. There is no guarantee that vulnerabilities which were discovered today, will exist tomorrow and the inverse is also true.
### Comprehensiveness
A penetration test should never guarantee the comprehensiveness of the test. Additional vulnerabilities may be present on applications and systems that were not discovered during the test.

## Support resources
* WSDL Web Services Descriptive Language
  * XML based document which describes the network services and endpoints.
* WADL/Web Application Descriptive Language
  * XML based document similar to WSDL, but is more lightweight but sufficient for documenting API and other https services.
* SOAP project file Simple Object Access Protocol
  * XML document which allows applications to communicate between each other regardless of operating system. Similar to REST.
* SDK documentation Software Development Kit
  * Documentation of the framework which was used to develop an application
* Swagger document
  * An easy to use and read REST API document
* XSD XML Schema Definition
  * Describes the structure of a document.
* Sample application requests
  * Recorded examples of transactions.
* Architectural diagrams
  * Helps define the relationship between multiple systems and applications.
