## records:
A	- Returns an IPv4 address of the requested domain as a result.
AAAA	- Returns an IPv6 address of the requested domain.
MX	- Returns the responsible mail servers as a result.
NS	- Returns the DNS servers (nameservers) of the domain.
TXT	- This record can contain various information. The all-rounder can be used, e.g., to validate the Google Search Console or validate SSL certificates. In addition, SPF and DMARC entries are set to validate mail traffic and protect it from spam.
CNAME -	This record serves as an alias for another domain name. If you want the domain www.hackthebox.eu to point to the same IP as hackthebox.eu, you would create an A record for hackthebox.eu and a CNAME record for www.hackthebox.eu.
PTR	- The PTR record works the other way around (reverse lookup). It converts IP addresses into valid domain names.
SOA- Provides information about the corresponding DNS zone and email address of the administrative contact.

```
dnsenum --dnsserver $target --enum <Domain>

dig soa $doamin

dig ns $doamin @$target
dig CH TXT $doamin @$target
dig any $doamin @$target
dig axfr $doamin @$target
dig axfr $doamin @$target

dnsenum --dnsserver $target --enum -p 0 -s 0 -o subdomains.txt -f /opt/useful/seclists/Discovery/DNS/subdomains-top1million-110000.txt inlanefreight.htb

```
