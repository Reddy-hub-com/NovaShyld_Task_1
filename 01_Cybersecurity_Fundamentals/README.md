Understanding CIA Triad
The CIA Triad is a fundamental framework in information security used to protect data and maintain secure, reliable systems. It guides policies to ensure information remains confidential, accurate and accessible to authorized users.
 Confidentiality
Confidentiality ensures that sensitive data is accessible only to authorized individuals or systems. Its purpose is to prevent unauthorized viewing, access or misuse of private information.
Risks to Confidentiality
•	Unauthorized Access: Attackers exploit vulnerabilities to access protected data.
•	Weak Encryption: Outdated or weak encryption can be easily broken, exposing sensitive information.
•	Insider Threats: Employees or trusted users may leak or accidentally expose confidential data.
Ensure Confidentiality
•	Encryption: Use strong encryption methods like AES or RSA to protect data from unauthorized reading. Avoid outdated algorithms like DES.
•	VPN: A Virtual Private Network creates an encrypted tunnel for internet communication, preventing interception
•	Access Controls: Implement strict authentication and authorization policies to limit data access to only authorized users.
 
Confidentiality
Integrity
Integrity ensures that data remains accurate, authentic and unaltered during storage or transmission. Any unauthorized modification or corruption compromises the reliability of data.
Risks to Integrity
•	Data Tampering: Attackers may intentionally alter or corrupt data for malicious purposes.
•	Malware & Ransomware: Malicious software can modify, encrypt or destroy data, leading to loss and system disruption.
Ensure Integrity
Hash Functions detects modifications by generating unique hash values for data. Common hash functions include
•	MD5: Produces a 128-bit hash value.
•	SHA Family: Includes SHA-1, SHA-2, SHA-3 with varying bit lengths.
Working of Hash Functions
•	Host A Sends Data: Host A creates a hash value (H1) using a hash function.
•	Attach Hash: H1 is sent along with the data.
•	Host B Verifies: Host B generates a new hash (H2) from the received data.
•	Compare: If H1 = H2, the data is unchanged (integrity preserved) else H1 ≠ H2, the data was altered or corrupted.
 
Hash Function
Note: Even a small change in the input (like altering a single word or character) will completely change the resulting hash.

Availability
Availability ensures that systems, networks and data are accessible to authorized users whenever needed. Disruptions can halt operations and cause major losses.
Risks to Availability
•	DoS and DDoS Attacks: Denial of Service (DoS) or Distributed Denial of Service (DDoS) attacks flood network resources with excessive traffic, making them unavailable to legitimate users.
•	Impact: Such attacks can cause major service disruptions, downtime and financial losses for companies.
Ensure Availability
 

To ensure availability, network administrators should focus on the following factors:
•	Hardware Maintenance: Regularly maintain and upgrade hardware to prevent failures and ensure smooth operations.
•	Regular Upgrades: Keep systems and software updated to maintain performance and security.
•	Failover Plan: Implement failover systems so that if one component fails, another can take over, minimizing downtime.
•	Preventing Bottlenecks: Monitor and manage network traffic to avoid congestion or bottlenecks, ensuring consistent performance.


A Few Examples of the CIA Triad
These real incidents show how gaps in confidentiality, integrity, or availability led directly to major consequences and why architecting your controls around the triad still matters.
Confidentiality breach
A healthcare staffing platform, ESHYFT, exposed over 86,000 records, complete with social security numbers, professional credentials, and scanned IDs, in a publicly accessible Amazon S3 bucket for months. There was no encryption or access control, and security researchers disclosed the exposure before the firm secured its cloud assets.
Integrity violation
Financial systems often pause file integrity checks during maintenance windows. One organization discovered that attackers had retroactively edited transaction logs on a billing system to hide fraudulent transfers. With integrity monitoring disabled during a patch cycle, the manipulation went undetected until discrepancies surfaced during reconciliation.
Availability failure
In London, hospitals served by Synnovis, a diagnostic laboratory for major NHS trusts, experienced significant disruptions after a ransomware attack shut down their IT systems. Over 1,500 surgical procedures and outpatient services were postponed. Systems remained offline for days, and clinical capacity dropped sharply.
These cases illustrate that data exposure, undetected tampering, or service unavailability is rarely accidental; it is the result of a missing or broken CIA control. When teams cannot point clearly to a failed leg of the triad, the response becomes slower, more expensive, and less effective.
In practice, designing around CIA does more than meet compliance; it helps prevent failures by making sure:
•	Confidentiality controls limit access and prevent public exposure
•	Integrity checks are continuous, not skipped during updates
•	Availability systems are exercise-tested, not assumed reliable
Mapping critical workflows: cloud storage, billing systems, and lab processing, to each pillar ensures that when something breaks, your team knows exactly what went wrong and where to fix it.

