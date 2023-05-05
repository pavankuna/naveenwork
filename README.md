An attacker would typically use a port scanner to assess what network services and ports are available on a given server. A port scanner is a software tool that can scan a range of IP addresses and port numbers to identify which ports are open and what services are running on those ports.

One of the Kali tools that can perform this function is Nmap (Network Mapper), which is pre-installed on Kali Linux. Nmap is a powerful and versatile port scanner that can be used to identify open ports, services running on those ports, and operating systems used by the target servers. It can perform a range of scan types, including TCP, UDP, SYN, and others, and can also perform service detection to determine the exact service running on a given port.

To scan a target server using Nmap, an attacker would typically open a terminal window on Kali Linux and use the following command:
nmap <target IP address or hostname>

   For example, to scan a server with the IP address 192.168.1.100, the attacker would use the following command:
   nmap 192.168.1.100
Nmap will then perform a default TCP scan of the server and report back which ports are open and what services are running on those ports. The attacker can then use this information to identify potential vulnerabilities and plan further attacks.
   
   Port scanning is a common technique used by attackers to identify what network services and ports are available on a given server, and Nmap is a popular tool used for this purpose that is pre-installed on Kali Linux.
