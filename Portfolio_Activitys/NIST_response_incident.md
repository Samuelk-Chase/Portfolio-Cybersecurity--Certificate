#### Incident Report Analysis

## Summary
- This afternoon there was an attack on a web design social media marketing buisnes server. The companys network services suddenly stoped responding causing sales to stop.The incident management team responded by blocking incoming ICMP packets and stopping all not critical netwrok services offline.The  malicious attacker overhelmed the company thorugh a DDos attack.The servers were offline for a totoal of two hours untill it was resoved and criticla netowrk services were restored. 

### Identify
- The incident managment team auditied the systems involved in the attack to find gaps in the security. The team found that the fire wall was not liminting the rate of incoming ICMP packts. The servers them selves were overwhelmed with the inflow of ICMP packets and all employees were not able to access what they needed to.

### Protect
The team has implemented new authentication policies to prevent future attacks including: 
- New firewall rule to limit the reate of incoming ICMP packets 
- Source IP address verification on the firewall ot check for spoofed IP addresses on incoming ICMP packets 
- Network monitoring software to dected abnormal traffic patterns 

### Detect
- The cybersecurity team configured source IP address verification on the firewall to check for spoofed IP addresses on incoming ICMP packets and implemented network monitoring software to detect abnormal traffic patterns.
### Respond
- For future security events, the cybersecurity team will isolate affected systems to prevent further disruption to the network. They will attempt to restore any critical systems and services that were disrupted by the event. Then, the team will analyze network logs to check for suspicious and abnormal activity. The team will also report all incidents to upper management and appropriate legal authorities, if applicable.

### Recover
- To recover from a DDoS attack by ICMP flooding, access to network services need to be restored to a normal functioning state. In the future, external ICMP flood attacks can be blocked at the firewall. Then, all non-critical network services should be stopped to reduce internal network traffic. Next, critical network services should be restored first. Finally, once the flood of ICMP packets have timed out, all non-critical network systems and services can be brought back online. 