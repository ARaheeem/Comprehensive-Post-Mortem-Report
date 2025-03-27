
<h1> Post Mortem Report</h1>


<h2>Description</h2>
This project involves the creation of a post-mortem report using a real life cybersecurity incident, aimed at identifying key factors leading to the breach, analysing the response efforts, and proposing measures to prevent future incidents. The report will cover the timeline of events, incident detection, mitigation strategies, communication channels, and lessons learned throughout the process. The goal is to provide a detailed analysis that helps improve incident response protocols, enhance security measures, and increase overall organisational resilience. The project will serve as an essential learning tool in identifying weaknesses, understanding the importance of effective communication, and building stronger defense mechanisms in the cybersecurity landscape.
<br />
<h2> Introduction </h2>
On 28/08/2018, British Airways website and mobile app were injected with malicious JavaScript into their payment processing page by Magecart hackers. The malicious code scanned payment details of British Airways customers in real time and sent them to an attacker-controlled server. This breach lasted until 05/09/2018 and resulted in data such as credit card numbers, CVVS and personal details of 380,000 customers to be compromised. 
<br />
<h2> Root cause Analysis</h2>
Attackers exploited a specific third-party script that was used on British Airways’ website. The malicious JavaScript was injected and used to steal payment detail of customers at checkout. The data was then sent over to a fake domain (the domain was called baways.com) setup by the hackers, which mimicked British Airways.The data breach was eventually detected by security researchers at RiskIQ because of suspicious code running on the British Airways website. Additionally, customers reported fraudulent transactions after booking flights. Data logs were then examined by British Airways security team to confirm the data exfiltration.
<br />
<h2> Summary of Event</h2>
<img src="https://i.imgur.com/sqY56vg.png" height="80%" width="80%" alt="image 1"/>
<br />
<img src="https://i.imgur.com/SyCHago.png" height="80%" width="80%" alt="image 2"/>
<br />
<h2>Incident detection and Escalation </h2>
Was the event detected within the expected timeframe? 

The event was detected within 24 hours and the malicious code was removed within 90 minutes, however there is room for improvement as early detection is crucial to minimise damage of cyber security incidents 

How was it detected? 

The detection was conducted by an external security team. The third-party cybersecurity firm noticed customer data was being sent to an unknown domain. The domain raised suspicions as it had no legitimate connection to British Airways. Additionally, customer data was being transmitted to external servers indicating a possible breach.  the JavaScript was discovered by the security team comparing British Airways code against previous iterations. 

 

How could time to detection be improved? 

British Airways could use real-time threat detection tools like SIEM systems (Splunk, ELK or IBM QRadar) to determine suspicious activity much quicker. Additionally, British Airways can implement stronger content security policies which would prevent unauthorised JavaScript executions. Regular Penetration testing and security audits can ensure vulnerabilities like this cannot be exploited in the future and greater compliance with security requirements. Furthermore, firewall can be introduced to detect malicious traffic much early to reduce response time. Implementation of Sub- resource Integrity can be used to ensure only trusted scripts run. 

How would you conform that the incident had been resolved? 

Testing and validation: British Airways should conduct through testing to ensure that all affected systems were clean and operational, and this may include validating backups, restoring data and verifying integrity of their domain. 
<br />
<h2>Takeaway/ Lesson learned  </h2>
British Airways data breach was a preventable cybersecurity incident caused by poor monitoring, weak security configurations. It also highlights the importance of monitoring network traffic, creating robust systems and investing in cybersecurity measures to minimise damage and response time. 
