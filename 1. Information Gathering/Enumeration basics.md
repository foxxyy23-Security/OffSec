# Port scanning

nmap:
nmap <scan types> <options> $target

-A 
	Aggressive - scans everything
-Pn 
	disables icmp echo requets treat host as online (used if machine does not respond to Ping)
-sU
	UDP port scan
-p-
	all ports65565
-p<port number>
	(-p80,443,22) scan only those ports
-sV
	- service scan
 --top-ports=10
	- scan the top 10 ports (can be changed)
--packet-trace
	- traces all packets sent and received 
-disable-arp-ping
--script
	runs specified scripts in target
### firewall/ids/ips bypass techniques 
-D RND:5
	-randomly generates 5 ips to appear as source address
-S
	- pick and choose source ip
--source-port 53
	- changes source port to 53

offical site:https://nmap.org/book/man-port-scanning-techniques.html

## SMB, ldap, Kerberos 
enum4linx -a $target

## LDAP
ldapsearch


##  HTTP/HTTPS
- Visit the site
	- click away and see what you can find
	- How does the application work?
	- any login pages?
		- User or admin
		- defult creds?


-web vulnerability scanning tools
	- Nikto
- Directory busting Tools
	- FFUF
	- Dirbuster
	- Dirb
	- Gobuster
	
