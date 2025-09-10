## external Pentest

### using certsh

```
curl -s https://crt.sh/\?q\=inlanefreight.com\&output\=json | jq . | grep name | cut -d":" -f2 | grep -v "CN=" | cut -d'"' -f2 | awk '{gsub(/\\n/,"\n");}1;' | sort -u

## sorting list m
for i in $(cat subdomainlist);do host $i | grep "has address" | grep inlanefreight.com | cut -d" " -f1,4;done
```
### subdomains
```
sublist3r -d $domain
```
owasp amass

tomnomnom 
### whois
```
whois $domain
```

### pull dns records 
```
 dig any $domain
```
DNS Record Enumeration: Query DNS for important records. For example, use dig or nslookup to find:
- A/AAAA records – host addresses for domain and subdomains (dig A example.com).
- NS records – name servers (dig NS example.com).
- MX records – mail exchangers (dig MX example.com) – check if they point to *.protection.outlook.com (indicates Office 365 email hosting)
- TXT records – especially SPF, DKIM, and DMARC (dig TXT example.com) to see email security configurations.
```
nslookup
```
### the harvester
```
theHarvester -d example.com -b google
```

### people
- public reords 
- job postings 
- linkedin 
- X

### getting email addresses
- hunter.io
- phonebook.cz
- Clear it
- google search

### getting passwords
Dehashed.com

- common password 
seasons 
company names
street namws 
nearby sports teams 

### other 
- github 

#### google fu
want specific site?
site: ___.com

subtract things 
(-) www

search for a file?
filetype: pdf, csv, docx etc


### confirming valid accounts
```
MailSniper

AADInternals
```
