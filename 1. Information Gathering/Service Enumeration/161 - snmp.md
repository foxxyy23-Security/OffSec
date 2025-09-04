

'''
snmpwalk -v2c -c public 10.129.14.128
'''



sudo apt install onesixtyone

onesixtyone -c /opt/useful/seclists/Discovery/SNMP/snmp.txt 10.129.14.128



sudo apt install braa
braa <community string>@<IP>:.1.3.6.*   # Syntax

braa public@10.129.14.128:.1.3.6.*
