### Example Cybersecurity Incident Report: Network Traffic Analysis

#### Part 1: Summary of the Problem Found in DNS and ICMP Traffic Log
   - The network protocol analyzer logs indicate that prot 53 is unreachable when attempting to access the website. Port 53 is usually used for DNS traffic. This may indicate a provlem with the server, meaning it could be down or experienceing connectivity issues. it is possible that this is an indication of a malicious attack on the server.



#### Part 2: Explanation of Analysis and Incident Details

- The incident occured at 1:24 pm when the company got phone call complaints stating that they were not able to access the client company website. The analyist responded and began running tests with the network protocol analyzer tool tcpdump. The resulting logs revealed that port 53, which is used for accessing domain names, was not reachable. We are continuing to investigate the root cause of the issue to determine how we can restore access to the secure web protal. Our next steps include varifying the DNS server and configuration, clearing DNS cache, then restarting our servers. The likely cause was due to DNS spoofing, where the hijacker may have created fake DNS records.

