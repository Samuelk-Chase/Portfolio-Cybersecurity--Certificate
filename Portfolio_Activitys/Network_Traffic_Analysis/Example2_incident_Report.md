### Example 2 Cybersecurity Incident Report: Analyze netowrk attacks 

#### Section 1: Identify the type of attack that may have caused this network interruption 
- One potential explanation for the website's connection timeout error message is an SYN flood attack.The logs show that there is an overwhelming amount of volume of incoming traffic, specifically SYN  requests. This could mean a malicious user is trying to use a DoS attack. 

#### Section 2: Explain how the attack is causing the website to malfunciton
- When website visitor try to establish connection wit hthe web server, a three-way handshake occurs using TCP protocol. 
1) The client sends a TCP request with a SYN flag to the server 
2) The server respons with a SYN and ACK flags 
3) Finally the client responds to the servers SYN-ACK segment with  only the ACK flag set.
- When the malicious actor sends a large number of SYN packets all at once, Upon recieving a SYN packet the target server allocates resources to create a half open connection and sends the SYN-ACK packet back to the spoofed Ip. Then because the packets dont have legitimate clients the server does not recieve the expected ACK flag response to complete the 3 way handshake the server remains open in a pending state consuming server resources causing the connection queue to fill up causing the server to become depleted of its resources. Thus making it so legitimage users can not use the server. The logs will usually show a pattern of TCP requests repetitivley over and over agin from the same spoofed IP address. 